
##Guest Book

kubectl apply -f redis-master-controller.json

kubectl apply -f redis-master-service.json

kubectl apply -f redis-slave-controller.json

kubectl apply -f redis-slave-service.json

kubectl apply -f guestbook-controller.json

kubectl apply -f guestbook-service.json

kubectl get services -o wide

kubectl delete rc/redis-master rc/redis-slave rc/guestbook svc/redis-master svc/redis-slave svc/guestbook