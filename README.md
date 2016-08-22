# **Ansible Role: Sudo**

[![Build Status](https://travis-ci.org/thiagomgo/ansible-role-sudo.svg?branch=master)](https://travis-ci.org/thiagomgo/ansible-role-sudo) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-sudo-blue.svg)](https://galaxy.ansible.com/thiagomgo/sudo/)

This role installs sudo and configure it by user.

## Requirements

This role only requires Ansible version 1.8+.

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

None

## Example Playbook

```yaml
---

- hosts: all

  vars:
    sudo: true
    sudo_user:
      - username

  roles:
    - ansible-role-sudo
```

## License

MIT / BSD

## Author Information

Thiago Gomes
- thiago.mgomes [at] gmail.com
