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

add model:
```bash
juju add-model development
```

Remove controller from cluster:
```bash
juju destroy-controller mycloud
```
