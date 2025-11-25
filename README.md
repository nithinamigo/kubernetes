# kubernetes

installed virtualbox in macos
dowloaded docker
start minikube:
minikube start --driver=docker
kubectl get nodes

list namespaces:
kubectl get namespaces

create namespaces:
kubectl create namespace dev
kubectl create namespace staging
kubectl create namespace prod

describe namespaces:
kubectl describe namespace dev

deploy inside namespaces:
kubectl create deployment nginx-deploy --image=nginx -n dev

expose namespaces:
kubectl expose deployment nginx-deploy --port=80 --type=NodePort -n dev


