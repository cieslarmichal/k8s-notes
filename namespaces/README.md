# Namespaces

Groups resources into logical units.

## Commands

kubectl get pods -n namespace-name

kubectl get pods --all-namespaces

kubectl create namespace development

## DNS

To access other service in different namespace: <service-name>.<namespace>.<service>.<domain>
Example: db-service.dev.svc.cluster-local
