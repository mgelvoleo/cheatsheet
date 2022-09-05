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
