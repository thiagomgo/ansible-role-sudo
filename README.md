# **Sudo**

This role installs sudo and configure it by user.

## Requirements
------------

None.

## Role Variables
--------------

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
------------

* Ansible >= 1.9

## Example Playbook
----------------

```yaml
---

- hosts: all

  vars:
    sudo: true|false
    sudo_user:
      - username

  roles:
    - thiagomgo.sudo
```

## License
-------

BSD

## Author Information
-------

Thiago Gomes <thiago.mgomes [at] gmail.com>


