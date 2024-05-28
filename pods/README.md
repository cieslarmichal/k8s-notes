# Pods

## Commands

kubectl apply -f pod-definition.yml

kubectl get pods -n namespace (-o wide)

kubectl delete pod <name>

kubectl run nginx --image=nginx

kubectl describe pod <name>

kubectl run redis --image=redis --dry-run=client -o yaml > redis.yaml

