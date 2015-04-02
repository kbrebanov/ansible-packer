packer
======

Installs Packer

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name             | Default                                                          | Description                  |
|------------------|------------------------------------------------------------------|------------------------------|
| packer_version   | 0.7.5                                                            | Version of Packer to install |
| packer_sha256sum | 8fab291c8cc988bd0004195677924ab6846aee5800b6c8696d71d33456701ef6 | SHA 256 checksum of package  |

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
