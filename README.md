# Getting Started

#### 1. docker build and create image
```
$ docker build -t learn/spring-boot-test:latest .
```

#### 2. apply and port-forwarding
```
$ kubectl apply -f k8s-deployment.yaml
$ kubectl apply -f k8s-service.yaml

$ kubectl port-forward service/spring-boot-test-loadbalancer-service 8080:8080
```


#### other
```
$ kubectl get all
$ kubectl get services
$ kubectl get pods
$ kubectl get deployments
$ kubectl scale deployment spring-boot-example --replicas=3
$ kubectl delete --all pods
$ kubectl delete --all deployments
$ kubectl delete --all namespaces
$ kubectl delete daemonsets,replicasets,services,deployments,pods,rc,ingress --all --all-namespaces

```