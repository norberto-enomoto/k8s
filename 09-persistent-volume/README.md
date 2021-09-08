# Comandos - 01-persistent-volume.yaml
- kubectl apply -f 01-persistent-volume.yaml
- kubectl get pv
- kubectl describe pv mysql-pv-volume

# Comandos - 02-persistent-volume-clain.yaml
- kubectl apply -f 02-persistent-volume-clain.yaml
- kubectl get pvc
- kubectl describe pvc mysql-pv-claim

# Comandos - 03-deployment-db.yaml
- kubectl apply -f 03-deployment-db.yaml
- kubectl get po -o wide

# Comandos - 04-deployment-app.yaml
- kubectl apply -f 04-deployment-app.yaml
- kubectl get po -o wide
- kubectl delete deployment hollowapp
- kubectl get po -o wide
- minikube tunnel

# Comandos para excluir o pod do mysql
- kubectl get po -o wide
- kubectl delete po <po-name>
- kubectl get po -o wide
- minikube tunnel