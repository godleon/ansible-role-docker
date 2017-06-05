[![Build Status](https://travis-ci.org/godleon/ansible-role-docker.svg?branch=master)](https://travis-ci.org/godleon/ansible-role-docker)


Role Name
=========

**godleon.docker**

Requirements
------------

## Software

- Python2.7
> sudo apt-get update && sudo apt-get -y install python2.7

Role Variables
--------------

The variables that should be passed to this role and a brief description about them are as follows:

```yaml
# Specify the users who can use docker commands without sudo
# You can keep it empty for root-only permission
docker_users:
  - user1
  - user2
  - user3
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- hosts: servers
  roles:
      - { role: godleon.docker }
```

License
-------

MIT

Author Information
------------------

**Leon Tseng** 

-  [godleon@GitHub](https://github.com/godleon)
