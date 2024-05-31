# Config maps

## Commands

kubectl create configmap app-config --from-literal=APP_COLOR=blue --from-literal=APP_MODE=prod

kubectl create configmap app-config --from-file=./path/to/config/file

kubectl get configmaps

kubect describe configmaps
