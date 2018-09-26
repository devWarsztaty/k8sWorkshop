kubectl rollout status deployments dumpster-deployment

kubectl rollout history deployment/dumpster-deployment

# find out what went wrong
kubectl rollout history deployment/dumpster-deployment --revision=X
kubectl rollout history deployment/dumpster-deployment --revision=X-1

kubectl rollout undo deployment/dumpster-deployment