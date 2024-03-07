# Step 2

Replace useless pod with a HTTP Service

Enter in one pod
```
kubectl exec --stdin --tty simple-pod-1 -n mooncard -- /bin/bash
```
Inside shell get the name of the running program (pid 1)
```
cat /proc/1/comm
```
Run curl
```
curl http://localhost
```