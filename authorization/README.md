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

kubectl api-resources --namespaced=true/false

kubectl get clusterroles

kubectl get clusterrolebindings

kubectl create clusterrole storage-admin --verb=list,create,get,watch --resource=persistentvolumes,storageclasses

kubectl create clusterrolebinding michal-storage-admin --clusterrole=storage-admin --user=michal
