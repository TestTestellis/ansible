# Ansible

[![Main](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml/badge.svg)](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml)

My personal ansible setup for my workstations and servers.

## Building

### Prerequisites

Make sure you have the following installed:

* [Python 3](https://www.python.org/downloads/)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/docs/installation)

Then install the Python requirements:

```shell
pip install -r requirements.txt
```

### Linting

Linting will run `yamllint` and `ansible-lint`:

```shell
molecule lint
```

### Building

Building creates the VMs and runs the playbook.

```shell
molecule converge
```

### Testing

Testing will lint, create the VMs, run the playbook and destroy the VMs.

```shell
molecule test
```
