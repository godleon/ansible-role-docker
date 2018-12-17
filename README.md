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

docker:
  # Specify the docker version(e.g. 17.03.2~ce-0~ubuntu-xenial). Ignore it if you want to install the latest version.
  version: "latest"
  # Specify the users(default is the user id you are using for doing ansible provision) who can use docker commands without sudo
  # You can keep it empty for root-only permission
  users:
    - ubuntu
```

And this role can also install the latest version of [Docker Compose](https://docs.docker.com/compose/overview/), if you want latest Docker Compose to be installed, you need to configure the variables as follows:

```yaml
docker:
  compose:
    install: true
  registry_mirror: "YOUR_REGISTRY_PROXY_URL"
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
