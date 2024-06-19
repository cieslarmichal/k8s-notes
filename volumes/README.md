# Volumes

Volumes allow to persist data when pod is down.

Persisted Volume is a cluster-wide storage pool of volumes to be used by Persisted Volume Claims to take a piece of Persisted Volume.

PVC is only bind to one PV, could be bound by labels (1 to 1 relation).

## Commands

kubectl get persistentvolume

kubectl get persistentvolumeclaim
