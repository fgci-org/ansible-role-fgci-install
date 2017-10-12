[![Build Status](https://travis-ci.org/CSCfi/ansible-role-fgci-install.svg)](https://travis-ci.org/CSCfi/ansible-role-fgci-install)
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

It is possible to install the ansible-pull-script as a systemd by setting:
<pre>
ansible_pull_systemd: True
</pre>

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
