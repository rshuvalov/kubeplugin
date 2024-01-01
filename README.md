## Metric plugin

### Enable metrics service
```
minikube addons enable metrics-server
```

### Move kubeplugin to the dir from PATH
```
cp scripts/kubeplugin ~/bin/kubectl-kubeplugin
```

### Run command
```
kubectl kubeplugin pods kube-system
```

Output example
```
pods, kube-system, coredns-5dd5756b68-ttb77, 4m, 67Mi
pods, kube-system, etcd-minikube, 42m, 151Mi
pods, kube-system, kube-apiserver-minikube, 89m, 473Mi
pods, kube-system, kube-controller-manager-minikube, 34m, 141Mi
pods, kube-system, kube-proxy-mj7vq, 1m, 75Mi
pods, kube-system, kube-scheduler-minikube, 6m, 75Mi
pods, kube-system, metrics-server-7c66d45ddc-r9ns6, 6m, 22Mi
pods, kube-system, storage-provisioner, 4m, 14Mi
```