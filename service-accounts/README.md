# Service accounts

When SA is created it generates token for the SA and then creates a secret object and stores token there. The secret is then linked to the SA.
Using describe command Tokens field is the name of the secret which stores JWT token.
Token can be used to make calls to Kubernetes API.

Each namespace has its own default SA, when pod is created the default SA with its token is automatically mounted to the pod as a volume mount.
Mounted in `/var/run/secrets/kubernetes.io/serviceaccount` inside the pod.
Default SA is very restricted, only permission to run basic API queries.

## Commands

kubectl create serviceaccount dashboard-sa

kubectl get sa

kubectl describe sa redis -n development
