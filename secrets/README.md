# Secrets

## Commands

kubectl create secret generic app-secret --from-literal=DB_HOST=mysql --from-literal=USER=root

kubectl create secret generic app-secret --from-file=<path>
