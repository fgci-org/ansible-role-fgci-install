[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-fgci-install.svg)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-fgci-install)
ansible-role-fgci-install
=========

Configures an FGCI install node

It does various things which are necessary - but in some cases could be moved to other roles.

 - installs EPEL
 - creates dhcp.d directory
 - creates nodes.conf for dhcpd
 - copy ansible hosts file to /var/www
 - copy ansible-pull-script.sh to /var/www
  - ansible-pull updates itself after it's done
 - copy in reinstall script

Requirements
------------


Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-fgci-install }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
