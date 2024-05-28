# Services

## Commands

kubectl expose pod redis --port=6379 --name redis-service --dry-run=client -o yaml

kubectl expose pod nginx --port=80 --name nginx-service --type=NodePort

kubectl create service clusterip --tcp=6379:6379

kubectl create service nodeport nginx --tcp=80:80 --node-port=30080

kubectl get svc
