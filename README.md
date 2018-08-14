linux defaultsoftware
=========

[![Build Status](https://travis-ci.org/ANTS-Framework/linux_defaultsoftware.svg?branch=master)](https://travis-ci.org/ANTS-Framework/linux_defaultsoftware)

Install software using yum or apt

Role Variables
--------------

```yml
    linux_defaultsoftware__yum_defaultsoftware:
        - vim
    linux_defaultsoftware__apt_defaultsoftware:
        - vim
```

Example Playbook
----------------


```yml
    - hosts: centos
      vars:
        - linux_defaultsoftware__yum_defaultsoftware: vim
      roles:
         - linux_defaultsoftware

    - hosts: ubuntu
      vars:
        - linux_defaultsoftware__yum_defaultsoftware:
            - vim
            - nginx
      roles:
         - linux_defaultsoftware
```

License
-------

GPLv3

Author Information
------------------
Part of the [ANTS Framework](https://ants-framework.github.io/)
