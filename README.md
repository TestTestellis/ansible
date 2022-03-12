# Ansible

[![Main](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml/badge.svg)](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml)

My personal ansible setup for my workstations and servers.

## Building

### Prerequisites

Software

* [Python 3](https://www.python.org/downloads/)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/docs/installation)

Python requirements:

```shell
pip install -r requirements.txt
```

### Linting

```shell
molecule lint
```

### Building

Create the VMs and run the playbook.

```shell
molecule converge
```

### Testing

Lint, create the VMs, run the playbook and destroy the VMs.

```shell
molecule test
```
