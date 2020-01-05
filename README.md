# snippets
Useful code snippets

## Kubernetes
### List all internal IP's in namespace
```sh
kubectl get nodes -o jsonpath='{.items[*].status.addresses[?(@.type=="InternalIP")].address}'
``` 
## Linux/unix
### sort ipv4 addresses
```sh
sort -n -t . -k 1,1 -k 2,2 -k 3,3 -k 4,4
```
