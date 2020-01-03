lb-tier
=======

Install HA proxy

Requirements
------------

Execute "base_config" role previously to enable Repository and install base tools and packages

Role Variables
--------------

- payload: haproxy

Dependencies
------------

handlers/main.yml --> restart service after some configuration change

Templates
---------

haproxy.cfg.j2 --> Configuration file por haproxy


Example Playbook
----------------

    - hosts: frontends
      roles:
         - {name: base-config, tags: base-config}
         - {name: lb-tier, tags: [lbs, haproxy]}

