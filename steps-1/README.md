# Step 1

Create a namespace and launch your first Pod

```
kubectl apply -f .
```

Observe pods
```
kubectl get pod
```
Nothing ?
```
kubectl get pod -a mooncard
```

Get detail about one Pod
```
kubectl describe pod simple-sleeping-pod -n mooncard
```

Get detail about other pod
```
kubectl describe pod simple-restarting-pod -n mooncard
```

Enter (shell) inside a running Pod
```
kubectl exec --stdin --tty simple-pod-1 -n mooncard -- /bin/bash
```