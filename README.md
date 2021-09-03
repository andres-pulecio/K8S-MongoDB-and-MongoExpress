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
##  Run service
```sh
kubectl apply -f mongo-secret.yaml
kubectl apply -f configmap.yaml
kubectl apply -f mongo.yaml
kubectl apply -f mongo-express.yaml
minikube service mongo-express-service
```

<!-- MARKDOWN LINKS & IMAGES -->
[overwiew-screenshot]: images/overview.png
[request-screenshot]: images/Request-flow.png


