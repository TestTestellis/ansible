# Ansible

[![Main](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml/badge.svg)](https://github.com/AkiKanellis/ansible/actions/workflows/main.yml)

My personal ansible setup for my workstations and servers.

## Building

### Prerequisites

Make sure you install the following:

* [Python 3](https://www.python.org/downloads/)
* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
* [Ansible Lint](https://ansible-lint.readthedocs.io/en/latest/installing.html)
* [Yamllint](https://yamllint.readthedocs.io/en/stable/quickstart.html)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [VirtualBox Extension Pack](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/docs/installation)
* [Molecule](https://molecule.readthedocs.io/en/latest/installation.html)

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
