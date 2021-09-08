# Comandos - 01-deployment-db.yaml
- kubectl apply -R -f 01-deployment-db.yaml
- kubectl get po -o wide
- kubectl logs -f <pod-name>
- kubectl describe pod <pod-name>
- kubectl get deployment
- kubectl describe deployment hollowdb
- kubectl get service
- kubectl get service hollowdb 

# Comandos - 02-secret.yaml
- kubectl apply -f 02-secret.yaml
- kubectl get secret
- kubectl describe secret hollow-secret

# Comandos - 03-deployment-app.yaml
- kubectl apply -f 03-deployment-app.yaml
- kubectl get po -o wide
- kubectl get deployment
- kubectl describe deployment hollowapp
- kubectl get ingress
- kubectl describe ingress hollowapp
- minikube tunnel

# Comandos para excluir o pod do mysql
- kubectl get po -o wide
- kubectl delete po <po-name>
- kubectl get po -o wide
- minikube tunnel