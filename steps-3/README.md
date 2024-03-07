# Step 3


```
kubectl apply -f steps-3
```

Immutable fields !

```
kubectl delete -f steps-2
kubectl apply -f steps-3
```

In a browser open : [http://simple-service.mooncard.svc.cluster.local/](http://simple-service.mooncard.svc.cluster.local/)

Observe Service type in 03-service.yaml : `ClusterIP`


    Exposes the Service on a cluster-internal IP. Choosing this value makes the Service only reachable from within the cluster. This is the default that is used if you don't explicitly specify a type for a Service. You can expose the Service to the public internet using an Ingress or a Gateway.

