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
| packer_version   | 0.8.1                                                            | Version of Packer to install |
| packer_sha256sum | b85451aa84f20264829916174267ae1642aec434e9a66c382d41e6c595be59d4 | SHA 256 checksum of package  |

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
