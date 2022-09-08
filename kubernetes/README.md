# Check the default 
```
Bash Command
minikube status
```

# Check the default 
```
Bash Command
kubectl config current-context
```

# Deploy applications
## Create a sample deployment and expose it on port 8080
```
Bash Command
kubectl create deployment hello-minikube --image=k8s.gcr.io/echoserver:1.4
```


```
Bash Command
kubectl expose deployment hello-minikube --type=NodePort --port=8080
```

## It may take a moment, but your deployment will soon show up when you run
```
Bash Command
kubectl get services hello-minikube
```
## The easiest way to access this service is to let minikube launch a web browser 
```
Bash Command
minikube service hello-minikube
```
## Halt the cluster
```
Bash Command
minikube stop
```

## Start the cluster
```
Bash Command
minikube start --driver=virtualbox [kvm,docker]
```

kubectl cluster-info


kubectl get nodes


kubectl get nodes


kubectl get pods

kubectl get namespaces

kubectl get pods --namespace=kube-system

## First Pods using nginx alpine
```
kubectl run nginx --image=nginx:1.23.1-alpine
```


kubectl desc pod


kubectl get pods -o wide

## Delate Pods
kubectl delete pod nginx

## Create deployment
kubectl create deployment nginx-deployment --image=nginx


kubectl get deployments

