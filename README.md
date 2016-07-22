apt
=========

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-apt.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-apt)

Install the dependendencies for the apt module.

http://docs.ansible.com/ansible/apt_module.html#requirements-on-host-that-executes-module

* python-apt
* aptitude(optional)

https://galaxy.ansible.com/suzuki-shunsuke/apt/

Requirements
------------

Nothing.

Role Variables
--------------

* apt_install_aptitude: Whether install aptitude or not. The default value is "no".
* apt_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
      - { role: suzuki-shunsuke.apt, apt_install_aptitude: yes }
```

License
-------

BSD
