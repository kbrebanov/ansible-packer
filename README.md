[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

packer
======

[![Ansible Role](https://img.shields.io/ansible/role/3297.svg)](https://galaxy.ansible.com/list#/roles/3297)

Installs Packer

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name             | Default                                                          | Description                  |
|------------------|------------------------------------------------------------------|------------------------------|
| packer_version   | 0.8.6                                                            | Version of Packer to install |
| packer_sha256sum | 2f1ca794e51de831ace30792ab0886aca516bf6b407f6027e816ba7ca79703b5 | SHA 256 checksum of package  |

Dependencies
------------

- kbrebanov.unzip

Example Playbook
----------------

Install Packer
```
- hosts: all
  roles:
    - { role: kbrebanov.packer }
```

Install Packer specifying version and checksum
```
- hosts: all
  roles:
    - { role: kbrebanov.packer, packer_version: 0.7.2, packer_sha256sum: 2e0a7971d0df81996ae1db0fe04291fb39a706cc9e8a2a98e9fe735c7289379f }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
