# Taints and Tolerations

Taints are applicable on nodes and set access restriction - pods must be tolerant to this restriction to be deployed there.
Toleration are applicable on pods and gives them access to be deployed on nodes.

## Commands

kubectl taint nodes node1 app=blue:(NoSchedule/PreferNoSchedule/NoExecute) - taint
kubectl taint nodes node1 blue:NoExecute- - untaint with hyphen in the end
