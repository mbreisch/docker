Docker Role
=========
[![Build Status](https://travis-ci.org/mbreisch/docker-role.svg?branch=master)](https://travis-ci.org/mbreisch/docker-role)

Installs docker-engine and docker-compose

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Variables:
* docker_authorized_user

Defaults:
* docker_ansible_module_support: yes

Dependencies
------------

There are no dependencies, but if you are using ufw you will need to configure some rules. TCP port 2375 should be opened for docker's use.
UFW's DEFAULT_FORWARD_POLICY should be set to "ACCEPT". You can Use mbreisch.ufw-role for docker's ufw configuration. 

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
