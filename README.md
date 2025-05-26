# For principal deployment metrics
kubectl port-forward svc/canary-demo 8080:80 -n canary-demo
curl http://localhost:8080/metrics > main-metrics.log
