Ansible Secure v. 0.0.2
=======================

[![CI](https://github.com/sv0/ansible-secure/actions/workflows/main.yml/badge.svg)](https://github.com/sv0/ansible-secure/actions/workflows/main.yml)

This ansible role installs the following tools and utils to harden server security:

* [chkrootkit](https://www.chkrootkit.org)
* [Rootkit Hunter](http://rkhunter.sourceforge.net)

It has been tested for the following Debian versions:

* Bullseye
* Bookworm

Requirements
------------

Ansible 2.14 version installed.

Variables
---------

```yaml

secure_rkhunter: true  # default value. install rkhunter

```

```yaml

secure_chkrootkit: true  # default value. install chkrootkit

```

```yaml

secure_ssh: false  # default value. do not modify ssd_config by befault

```

Example Playbook
----------------

```yaml
  - hosts: servers
    roles:
      - role: sv0.secure
```

License
-------

MIT

Author Information
------------------

[Slavik Svyrydiuk](https://slavik.svyrydiuk.eu/about.html)
