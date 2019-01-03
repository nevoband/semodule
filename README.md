Role Name
=========

This role allows to create, compile and include SELinux modules
This is a copy of https://github.com/MWojtowicz/ansible-semodule 
I simply added my own template to the module for shibboleth

Requirements
------------

It requires Development tools (`yum groupinstall "Development tools"`)

Role Variables
--------------

#SELinux Settings
selinux_modules:
  - name: mod_shib-to-shibd

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: semodule }

License
-------

MIT
