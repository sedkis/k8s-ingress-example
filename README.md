# Tyk OSS Deployment

Deploying Tyk as an ingress, with a bunch  of APIs it is reverse proxying to.
`part-2` folder has an ELK and Tyk Pump deployment for analytisc.

1. Create a new namespace
```
$ kubectl create ns apps
```


2. Deploy APIs and API Gateway into namespace

```
$ kubectl apply -f . -n apps

deployment.apps/another-api created
service/another-api created
configmap/tyk-apis created
deployment.apps/tyk-gtw created
service/tyk-svc created
deployment.apps/my-rest-api created
service/my-rest-api created
deployment.apps/redis created
service/redis created
deployment.apps/third-api created
service/third-api created
```
