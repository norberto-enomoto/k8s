# https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale-walkthrough/

# Comandos
- minikube addons enable metrics-server
- kubectl apply -f https://k8s.io/examples/application/php-apache.yaml
- kubectl autoscale deployment php-apache --cpu-percent=50 --min=1 --max=10
- kubectl get hpa
- kubectl run -i --tty load-generator --rm --image=busybox --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"

# Abrir um outro terminal
- watch kubectl get hpa

# Abrir um outro terminal
- watch kubectl get deployment php-apache

# Abrir um outro terminal
- watch kubectl get po -o wide
