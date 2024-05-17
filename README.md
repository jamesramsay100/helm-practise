# Create cluster

```shell
minikube start --vm-driver=hyperkit
```

```shell
minikube status 
```

```shell
kubectl get all
```

# Install chart
```shell
helm install my-mongo-release ./my-mongo-chart
```
```shell
 kubectl get pods --watch
```

```shell
kubectl port-forward svc/mongo-express 8081:8081
```

# Other
After making a change (e.g. replicaCount: 1 -> 2)
```shell
helm upgrade my-mongo-release ./my-mongo-chart
```
```shell
helm rollback my-mongo-release [REVISION]
```
```shell
helm history my-mongo-release
```

# Shut down
```shell
helm uninstall my-mongo-release
```
