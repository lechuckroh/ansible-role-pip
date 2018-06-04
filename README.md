# Ansible role `pip`

An ansible role for PIP

Tested under:
* CentOS 7.4

## Requirements

No requirements

## Role Variables

| Variable               | Default | Comments                |
|:-----------------------|:--------|:------------------------|
| `pip_version`          | `2`     | set `3` to install PIP3 |
| `pip_install_packages` | `[]`    | PIP packages to install. See [PIP module](http://docs.ansible.com/ansible/latest/modules/pip_module.html#pip-module) |

## Dependencies

No dependencies

## Example Playbook

```yaml
---
- name: example
  hosts: all
  become: true
  vars:
    pip_version: 2
    pip_install_packages: ['lxml']
  roles:
  - lechuckroh.pip
```

## License
MIT
