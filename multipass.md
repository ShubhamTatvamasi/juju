# multipass

Setup a new charm development cluster:
```bash
multipass launch charm-dev \
  --name charm-dev
```

Access Shell for the VM:
```bash
multipass shell charm-dev
```

Delete VM:
```bash
multipass delete --purge charm-dev
```
