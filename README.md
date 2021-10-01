# juju

https://juju.is/docs/sdk/dev-setup

Check your kubernetes cluster name:
```bash
kubectl config get-contexts
```

Install Juju controller on your kubernetes cluster:
```bash
juju bootstrap local mycloud
```
> This is install controller in `controller-mycloud` namespace

check status for controller:
```bash
juju status
```

add model (this will create new namespace):
```bash
juju add-model development
```

list all models:
```bash
juju models
```

switch model:
```bash
juju switch development
```

deploy the charm:
```bash
juju deploy ./hello-kubecon.charm --resource gosherve-image=jnsgruk/gosherve
```

watch juju status:
```bash
watch -n 1 juju status
```


Remove controller from cluster:
```bash
juju destroy-controller mycloud
```

juju debug logs:
```bash
juju debug-log
```

