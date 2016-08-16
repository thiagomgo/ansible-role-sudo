# **Ansible Role: Sudo**

[![Build Status](https://travis-ci.org/thiagomgo/ansible-role-sudo.svg?branch=master)](https://travis-ci.org/thiagomgo/ansible-role-sudo)

This role installs sudo and configure it by user.

## Requirements

None.

## Role Variables

Here is a list of all the default variables for this role, which are also available in `defaults/main.yml`.

```yaml
---

# enable sudo
sudo: true

# package name (version)
sudo_package: sudo

# username
sudo_user: []

```

## Dependencies

* Ansible >= 1.9

## Example Playbook

```yaml
---

- hosts: all

  vars:
    sudo: true
    sudo_user:
      - username

  roles:
    - thiagomgo.sudo
```

## License

BSD

## Author Information

Thiago Gomes
- thiago.mgomes [at] gmail.com


