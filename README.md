# juju

Check your kubernetes cluster name:
```bash
kubectl config get-contexts
```

Install Juju controller on your kubernetes cluster:
```bash
juju bootstrap local
```

Remove controller from cluster:
```bash
juju destroy-controller local
```
