Docker Role
=========
[![Build Status](https://travis-ci.org/mbreisch/docker-role.svg?branch=master)](https://travis-ci.org/mbreisch/docker-role)

Installs docker-engine and docker-compose

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

UFW is expected but not required.

Defaults:
* docker_ufw: yes

Dependencies
------------

Uses mbreisch.ufw-role for docker ufw configuration. TCP port 2375 is opened for docker's use.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
