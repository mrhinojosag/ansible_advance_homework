base-config
===========

Configure Repository and Install base tools and packages

Template
--------

open_three-tier-app.repo --> Repository for RHEL7

Example Playbook
----------------

    - hosts: servers
      roles:
         - {name: base-config, tags: base-config}

