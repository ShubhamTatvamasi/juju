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

### Containerd

Download nerdctl tool for managing containerd images:
```bash
wget https://github.com/containerd/nerdctl/releases/download/v1.0.0/nerdctl-1.0.0-linux-arm64.tar.gz
tar -xf nerdctl-1.0.0-linux-arm64.tar.gz
rm nerdctl-1.0.0-linux-arm64.tar.gz
```

