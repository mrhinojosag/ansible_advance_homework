db-tier
=======

Install postgressql server Data Base

Requirements
------------

Execute "base_config" role previously to enable Repository and install base tools and packages

Example Playbook
----------------

    - hosts: appdbs
      roles:
         - {name: base-config, tags: base-config}
         - {name: db-tier, tags: [dbs, postgres]}


