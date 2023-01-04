# Minikube Sandbox

## Start minikube

```bash
minikube start
```

```bash
minikube start --cpus 2 --memory 2G --nodes 2
```

## Delete minikube

```bash
minikube delete
```

## Jobs

### Apply

```bash
kubectl apply -f jobs
```

### Delete

```bash
kubectl delete -f jobs
```

### Shell on kubepod

```bash
kubectl exec kubepod kubectl -it -- sh
```
