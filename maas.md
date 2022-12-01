# MAAS


Add MAAS Cloud type and cloud name: `maas`:
```bash
juju add-cloud
```
> `http://192.168.20.23:5240/MAAS`

Add credentials for maas:
```bash
juju add-credential maas
```

Setup maas cloud:
```bash
juju bootstrap maas maasCloud
```

