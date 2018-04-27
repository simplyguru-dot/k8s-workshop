# hello-node simple application

eval $(minikube docker-env)

docker build -t hello-node:v1 .

docker images

kubectl run hello-node --image=hello-node:v1 --port=8080


kubectl get pods

kubectl get deployments

kubectl expose deployment hello-node --type=NodePort

kubectl get services

curl $(minikube service hello-node --url)

kubectl delete service,deployment hello-node

minikube stop
