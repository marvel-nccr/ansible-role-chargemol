[![Build Status](https://travis-ci.org/marvel-nccr/ansible-role-chargemol.svg?branch=master)](https://travis-ci.org/marvel-nccr/ansible-role-chargemol)

# Ansible Role: marvel-nccr.chargemol

An Ansible role that installs the [chargemol](https://sourceforge.net/p/ddec) program for computing DDEC atomic charges on Ubuntu.

## Installation

`ansible-galaxy install marvel-nccr.chargemol`

## Role Variables

See `defaults/main.yml`

## Example Playbook

```yaml
- hosts: servers
  roles:
  - role: marvel-nccr.chargemol
```

## Development and testing

This role uses [Molecule](https://molecule.readthedocs.io/en/latest/#) and [Docker](https://www.docker.com/) for tests.

After installing [Docker](https://www.docker.com/):
```
git clone https://github.com/marvel-nccr/ansible-role-chargemol marvel-nccr.chargemol
# Note: folder name marvel-nccr.chargemol is required for running tests
cd marvel-nccr.aiida
pip install -r requirements.txt  # Installs molecule
molecule test  # runs tests

## License

MIT

## Contact

Please direct inquiries regarding Quantum Mobile and associated ansible roles to the [AiiDA mailinglist](http://www.aiida.net/mailing-list/).
