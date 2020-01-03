config-tower
============

Configure ansible tower job templates and workflow

Role Variables
--------------

- vars/main.yml

Dependencies
------------

- tasks/pre-config-tower.yml
- tasks/post-config-tower.yml
- tasks/ec2_dynamic.yml
- tasks/job_template.yml
- tasks/workflow_template.yml

Example Playbook
----------------

    - hosts: localhost
      roles:
         - config-tower

