# Step 6


Remove individual pods

```
kubectl delete pod/simple-pod-1 -n mooncard
kubectl delete pod/simple-pod-2 -n mooncard
```

Deploy pod via a deployment
```
kubectl apply -f steps-6
```
