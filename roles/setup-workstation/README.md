setup-workstation
=================

Setup workstation, create network, ssh keypair, security group etc.

Requirements
------------

Request the following environments

- Ansible Advanced - Homework

- Ansible Advanced - OpenStack

Role Variables
--------------

vars/main.yml

Dependencies
------------

main.yml include the followind files:

- tasks/pre-tasks.yml
- tasks/create-flavor.yml
- tasks/create-keypair.yml
- tasks/create-sg.yml
- tasks/create-image.yml
- tasks/create-network.yml

site-setup-workstation.yml include the following file:

- site-install-isolated-node.yml 


Example Playbook
----------------

    - hosts: workstation
      become: yes
      roles:
        - setup-workstation

