# Deployments

Deployments contain replicasets and pods.

## Commands

kubectl get all

kubectl get deployments

kubectl describe pod pod-name

kubectl create deployment httpd-frontend --image=httpd:2.4-alpine --replicas=3
