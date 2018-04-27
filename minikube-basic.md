## Minikube basic operations

minikube start

minikube dashboard



kubectl run hello-minikube --image=k8s.gcr.io/echoserver:1.4 --port=8080

kubectl expose deployment hello-minikube --type=NodePort

kubectl get pod

curl $(minikube service hello-minikube --url)

kubectl delete service hello-minikube

kubectl delete deployment hello-minikube

minikube stop