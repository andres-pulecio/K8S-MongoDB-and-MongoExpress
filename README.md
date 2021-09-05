# About The Project
This is a Demo Project of K8S using Mongo DB and Mongo Express:

## Overview
[![Overview Screen Shot][overwiew-screenshot]](https://www.youtube.com/watch?v=X48VuDVv0do)
## Request Flow
[![Request Flow Screen Shot][request-screenshot]](https://www.youtube.com/watch?v=X48VuDVv0do)


## Create minikube cluster
```sh
minikube start 
kubectl get nodes
minikube status   
kubectl version
```
##  Create Namespace "my-namespace"
```sh
kubectl create namespace my-namespace
```
##  Run service
```sh
kubectl apply -f mongo-secret.yaml -n my-namespace
kubectl apply -f configmap.yaml -n my-namespace
kubectl apply -f mongo.yaml -n my-namespace
kubectl apply -f mongo-express.yaml -n my-namespace
minikube service mongo-express-service -n my-namespace
```

<!-- MARKDOWN LINKS & IMAGES -->
[overwiew-screenshot]: images/overview.png
[request-screenshot]: images/Request-flow.png


