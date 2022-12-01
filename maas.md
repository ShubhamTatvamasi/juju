# MAAS


Add MAAS Cloud type `maas` and cloud name: `maas-cloud`:
```bash
juju add-cloud
```
> endpoint url: `http://192.168.20.23:5240/MAAS`

Add credentials for maas:
```bash
juju add-credential maas-cloud
```

Setup maas cloud:
```bash
juju bootstrap maas-cloud
```

Remove Cloud:
```bash
juju remove-cloud maas-cloud
```
