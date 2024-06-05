Secure
======

[![CI](https://github.com/sv0/ansible-secure/actions/workflows/main.yml/badge.svg)](https://github.com/sv0/ansible-secure/actions/workflows/main.yml)

This ansible role installs the following tools and utils to harden server security:

* [Rootkit Hunter](http://rkhunter.sourceforge.net)

It has been tested for the following Debian versions:

* Buster
* Bullseye
* Bookworm

Requirements
------------

Ansible 2.14 version installed.

Variables
---------

```yaml

secure_rkhunter: true  # default, defines install or not rkhunter

```

Example Playbook
----------------

Including an example of how to use your role (for instance, with
variables passed in as parameters) is always nice for users too:

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
