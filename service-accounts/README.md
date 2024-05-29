# Service accounts

Using describe command Tokens field is the name of the secret which stores JWT token.
Token can be used to make calls to Kubernetes API.

Each namespace has its own default SA, when pod is created the default SA with its token is automatically mounted to the pod as a volume mount.
Mounted in `/var/run/secrets/kubernetes.io/serviceaccount` inside the pod, there are 3 files: ca.crt, namespace and token.

## Commands

kubectl create serviceaccount dashboard-sa

kubectl create token dashboard-sa - creates jwt token

kubectl get sa

kubectl describe sa redis -n development
