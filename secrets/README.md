# Secrets

Secret values must be base64 encoded

## Commands

kubectl get secrets

kubectl get secret app-secret -o yaml

kubectl describe secrets

kubectl create secret generic app-secret --from-literal=DB_HOST=mysql --from-literal=USER=root

kubectl create secret generic app-secret --from-file=path

echo -n 'mysql' | base64

echo -n 'bXlzcWw=' | base64 --decode
