# Step 4

```
brew install mkcert
brew install nss
mkcert -install
mkcert  "*.local.mooncard.co" localhost 127.0.0.1 ::1
kubectl create secret tls localdev --key _wildcard.local.mooncard.co+3-key.pem --cert _wildcard.local.mooncard.co+3.pem -n ingress-nginx
```

Add an entry in /etc/hosts
```
127.0.0.1    nginx.local.mooncard.co
```


```
kubectl apply -f steps-4
```