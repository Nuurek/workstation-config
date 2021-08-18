# Workstation Config by Nuurek

## Workstation setup

### Install required packages
```
sudo apt update
sudo apt upgrade
sudo apt install -y git
```

### Install Ansible
```
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install -y ansible
```

### Run the Ansible using the configuration pulled from GitHub

```
ansible-pull --url https://github.com/Nuurek/workstation-config.git
```

## Development

### Create virtual environment and activate it

```
python3 -m venv .venv && source .venv/bin/activate
```

### Install required packages

```
pip install -r requirements.txt
```

### Run the work in progress version of the playbook

```
ansible-playbook local.yml
```
