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
kubectl create deployment hello-minikube --image=k8s.gcr.io/echoserver:1.4 -n dev
kubectl get pods -n dev
k get pods --all-namespaces


```

```
Bash Command
kubectl expose deployment hello-minikube --type=NodePort --port=8080

or

k expose deployment hello-minikube --type=LoadBalancer --port=8080 -n dev
```

## It may take a moment, but your deployment will soon show up when you run
```
Bash Command
kubectl get services hello-minikube
k get services -n dev
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

## Delete Pods
kubectl delete pod nginx

## Create deployment
kubectl create deployment nginx-deployment --image=nginx


kubectl get deployments

## schedule disable
kubectl cordon minikube

#schedule disable
kubectl cordon minikube


kubectl get namespace


kubectl create namespace prod

## Create namespace using manifest yml
k create -f namespace-prod.yam

k describe namespace prod

## Display Event of namespace dev
k get events -n dev


## Make default namespace
kubectl config set-context --current --namespace=dev

## Create a deployment using manifest file
k apply -f v1.yaml

## Delete a deployment using manifest file
k delete -f v1.yaml

## Display the replica 
k get replicaset

## Display the logs of the pods and a live activity
k logs -l app=mywebapp

k logs -f -l  app=mywebapp

## Restart Pods
k rollout restart deployment mydeployment

## Drain Pods
k drain minikube --ignore-daemonsets=true --force
