# Commandos - 01-deployment-db.yaml
- kubectl apply -R -f 01-deployment-db.yaml
- kubectl get po -o wide
- kubectl logs -f <pod-name>
- kubectl describe pod <pod-name>
- kubectl get deployment
- kubectl describe deployment hollowdb
- kubectl get service
- kubectl get service hollowdb 

# Comandos - 02-configmap.yaml
- kubectl apply -f 02-configmap.yaml
- kubectl get configmap
- kubectl describe configmap hollow-config

# Comandos - 03-pod.yaml
- kubectl apply -f 03-pod.yaml
- kubectl get po -o wide
- kubectl exec -it shell-demo -- /bin/bash
- echo $DATABASE_URL
- exit

# Comandos - 04-deployment-app.yaml
- kubectl apply -f 04-deployment-app.yaml
- kubectl get po -o wide
- kubectl get deployment
- kubectl describe deployment hollowapp
- kubectl get ingress
- kubectl describe ingress hollowapp
- minikube tunnel
