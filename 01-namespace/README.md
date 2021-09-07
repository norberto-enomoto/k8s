- kubectl apply -f namespace.yaml
- kubectl get namespaces
- kubectl get pods -o wide --all-namespaces
- kubectl get pods -o wide
- kubectl get pods -o wide -n dxc-namespace
- kubectl get po -o wide -n dxc-namespace --show-labels
- kubectl describe pod nginx -n dxc-namespace
- kubectl logs nginx -n dxc-namespace
- kubectl logs -f nginx -n dxc-namespace
 