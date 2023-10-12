# WIP

### Why do we need litmus-chaos?

To help teams find problems and possible system breakdowns by safely running tests that create controlled chaos in their infrastructure. (1*)

### Prerequisites (2*)

- Kubernetes 1.17 or later (Let's install v1.25.14)

  - minikube (installation)
     - ```curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64```
     - ```sudo install minikube-linux-amd64 /usr/local/bin/minikube```
  - ```minikube start --memory 4096 --cpus 4 --kubernetes-version v1.25.14```
  - ```minikube addons enable metrics-server``` 

- A Persistent volume of 20GB

   - NOTE: Recommend to have a Persistent volume(PV) of 20GB, You can start with 1GB for test purposes as well. This PV is used as persistent storage to store the chaos config and chaos-metrics in the Portal. By default, litmus install would use the default storage class to allocate the PV. Provide this value

- Helm3 or kubectl

### Installation 

- 

### Test (Chaos Experiments)


### Resources
1*. https://litmuschaos.io/

2*. https://docs.litmuschaos.io/docs/getting-started/installation