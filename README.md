# Basic Kubernetes Deployment Demo
## Getting started
For this project I strongly recommend installing minikube to get up and running quickly.  
(Installation guide (https://minikube.sigs.k8s.io/docs/start/)) 

The command 'brew install minikube' will install both minikube and kubectl (kubectl is vital for the commands below).  

Start a cluster using the command 'minikube start --driver=docker' (docker can be replaced by whichever hypervisor you've opted for).

## Start up commands 
$ kubectl apply -f mongo-secret.yml

$ kubectl apply -f mongo.yml

$ kubectl apply -f mongo-configmap.yml

$ kubectl apply -f mongo-express.yml

$ minikube service mongo-express-service  

## Additional commands
Generate username secret:  
$ echo -n 'username' | base64  

Generate password secret:  
$ echo -n 'password' | base64

