# Deployments

Deployments contain replicasets and pods.

Two types of deployments: recreate and rolling update.

## Commands

kubectl get all

kubectl get deployments

kubectl describe pod pod-name

kubectl create deployment httpd-frontend --image=httpd:2.4-alpine --replicas=3

kubectl rollout status deployment my-deployment

kubectl rollout history deployment my-deployment

kubectl rollout undo deployment my-deployment

kubectl rollout history deployment nginx --revision=1

kubectl rollout history deployment nginx --revision=3

kubectl rollout undo deployment nginx --to-revision=1
