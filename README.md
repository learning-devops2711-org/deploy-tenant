## Reload Nginx
kubectl exec -n nginx $(kubectl get pods -n nginx -o jsonpath='{.items[0].metadata.name}') -- sh -c 'nginx -t && nginx -s reload'



