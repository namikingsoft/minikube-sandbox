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

## Web

### Apply

```bash
kubectl apply -f web
```

### Delete

```bash
kubectl delete -f web
```

### Tunnel

```bash
minikube service nginx1
```

## Namespaces

### Apply

```bash
kubectl apply -f namespaces
```

### Delete

```bash
kubectl delete -f namespaces
```

### Switch namespace

```bash
kubectl config set-context $(kubectl config current-context) --namespace=production
```

```bash
kubectl config set-context $(kubectl config current-context) --namespace=staging
```

```bash
kubectl config set-context $(kubectl config current-context) --namespace=default
```

### Show current namespace

```bash
kubectl config get-contexts
```
