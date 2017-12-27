Extra Repositories
==================

Adds the EPEL, IUS, and Remi repositories to CentOS or RedHat.

Installs layman, adds overlays, and syncs new overlays for Gentoo systems.

Requirements
------------

None.

Role Variables
--------------

For Red Hat based systems:
```yml
repository_install_epel: True
repository_install_ius: False
repository_install_remi: True
```

For Gentoo systems:
```yml
extra_repositories_layman_overlays:
  - java
  - pentoo
```

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: all
  roles:
    - { role: the-paulus.extra-repositories }

- hosts: all
  roles:
    - role: the-paulus.extra-repositories 
```

License
-------

BSD
