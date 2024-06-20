# Authorization

## Commands

kubectl get roles

kubectl get rolebindings

kubectl describe role developer

kubectl describe rolebindings developer-binding

kubectl auth can-i create-deployments

kubectl auth can-i delete-nodes

kubectl auth can-i create-deployments --as dev-user
