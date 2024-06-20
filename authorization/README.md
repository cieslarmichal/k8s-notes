# Authorization

## Commands

kubectl config view

kubectl get roles

kubectl get rolebindings

kubectl describe role developer

kubectl describe rolebindings developer-binding

kubectl auth can-i create-deployments

kubectl auth can-i delete-nodes

kubectl auth can-i create-deployments --as dev-user --namespace test

kubectl create role developer --verb=list,create,delete --resource=pods

kubectl create rolebinding dev-user-binding --role=developer --user=dev-user
