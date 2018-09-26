kubectl rollout status deployments dumpster-deployment

kubectl rollout history deployment/dumpster-deployment

# find out what went wrong
kubectl rollout history deployment/dumpster-deployment --revision=X
kubectl rollout history deployment/dumpster-deployment --revision=X-1

kubectl set image deployment/dumpster-deployment dumpster-deployment-container=gutek/dumpster:0.5