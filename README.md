# MongoDB-deployment-on-minkube

kubectl create -f mongodata-persistentvolumeclaim.yaml
kubectl create -f mongodb-deployment.yaml
kubectl expose deployment mongodb --type LoadBalancer
minikube service mongodb
mongo --host <minikube-ip> --port <five-digit-port>
