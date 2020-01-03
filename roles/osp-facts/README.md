osp-facts
=========

Generate in-memory inventory for OSP instances

Example Playbook
----------------

    - hosts: workstation
      gather_facts: true
      roles:
      - name: osp-facts
