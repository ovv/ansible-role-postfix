ovv.postfix
===========

[![Build Status](https://travis-ci.org/ovv/ansible-role-postfix.svg?branch=master)](https://travis-ci.org/ovv/ansible-role-postfix)

Ansible role to install and configure Postfix.

Installation
------------

To install this roles clone it into your roles directory.

```bash
$ git clone https://github.com/ovv/ansible-role-postfix.git ovv.postfix
```

If your playbook already reside inside a git repository you can clone it by using git submodules.

```bash
$ git submodule add -b master https://github.com/ovv/ansible-role-postfix.git ovv.postfix
```

Role Variables
--------------

* `mailname`: Server name
* `mail_aliases`: Dict of alias to add.

Example Playbook
----------------

```yaml

- hosts: localhost
  roles:
    - ovv.postfix
  vars:
    mailname: example.com
    mail_aliases:
      root: root@example.com
```

License
-------

MIT
