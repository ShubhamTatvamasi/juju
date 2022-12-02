# juju

https://juju.is/docs/sdk/dev-setup

https://juju.is/tutorials

Juju Dashboard tunnel:
```bash
ssh -L 17070:10.30.1.128:17070 -N ubuntu@192.168.21.2
```

https://localhost:17070/dashboard/

---

Setup **ARM** architecture:
```bash
juju set-model-constraints arch=arm64
```

List all Juju controllers:
```bash
juju controllers
```

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


