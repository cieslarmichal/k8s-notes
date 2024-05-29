# Pods

## Commands

kubectl apply -f pod-definition.yml

kubectl get pods -n namespace (-o wide)

kubectl delete pod <name>

kubectl run nginx --image=nginx

kubectl describe pod <name>

kubectl run redis --image=redis --dry-run=client -o yaml > redis.yaml

kubectl get pod webapp -o yaml > my-new-pod.yaml - extracts pod definition

kubectl edit deployment my-deployment

kubectl exec ubuntu-sleeper -- whoami
