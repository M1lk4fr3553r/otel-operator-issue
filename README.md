# Demo chart to show pod injection not working when the cluster starts up

## Prerequisites
``` bash
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.14.4/cert-manager.yaml
```

## Install
``` bash
helm dep update otel-operator && helm package otel-operator && helm install otel-operator otel-operator-0.1.0.tgz
```
