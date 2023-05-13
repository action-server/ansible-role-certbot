ansible-role-certbot
=========

Ansible role to install and configure certbot, and generate an ssl certificate.

Requirements
------------

Host must have python and an ssh key configured.

It also only works with the nginx at the moment, so make sure it's installed and configured!

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: certbot
           domain_names: [ 'www.example.com', 'example.com' ]
           cert_name: example_cert_name
           cert_email: example@example.com


License
-------

GNU General Public License v3.0
