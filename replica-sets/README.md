# Replica sets

## Commands

kubectl get replicationcontroller / rc

kubectl get replicaset / rs

kubectl scale -f replicaset-definition.yml --replicas=6 

kubectl scale replicaset <name> --replicas=6

kubectl describe replicaset <name>

kubectl explain replicaset

kubectl edit rs <name>
