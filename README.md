# Configuration

This repository contains Ansible playbook for configuring local development machines that run Ubuntu 22.

## Setup

Install Ansible:
```
sudo apt install ansible
```

## Machines

The repository contains common tasks for all machines as well as playbooks for specific machines. Currently available, machine-specific, playbooks:

* `workstation`

## Secrets

Put all the required secrets under `secrets/` directory in this repository. The structure of that directory must be like that:

* `.ssh`
* `.aws`
* `JetBrains/`
    * `Pycharm20xx.y/`
    * `CLion20xx.y/`
    * etc.

## Running the playbook

Run the playbook `sudo ansible-playbook {machine}.yaml`
