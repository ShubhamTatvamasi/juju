# charmcraft

https://juju.is/docs/sdk/hello-world

install charmcraft (Ubuntu only):
```bash
sudo snap install charmcraft --classic
```

start fresh operator:
```bash
mkdir hello-kubecon; cd hello-kubecon
charmcraft init
```

---

install virtualenv:
```bash
# for macOS
pip3 install virtualenv

# for Ubuntu
sudo apt install -y python3-virtualenv python3-pip
```

create virtual environment:
```bash
virtualenv venv
```

activate virtual environment:
```bash
source venv/bin/activate

# come out of virtual environment
deactivate
```

Install dependencies:
```bash
pip3 install -r requirements-dev.txt
```

---

build the charm:
```bash
charmcraft pack

# You have have to run this command before the above command.
lxd init --auto
```

