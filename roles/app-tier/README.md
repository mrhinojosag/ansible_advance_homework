app-tier
=========

Install application server Tomcat

Requirements
------------

Execute "base_config" role previously to enable Repository and install base tools and packages

Role Variables
--------------

- payload: tomcat

- tomcat_web_root: /usr/share/tomcat/webapps/ROOT

Dependencies
------------

handlers/main.yml  --> restart service after some configuration change

Templates
---------

index.html.j2 --> Html page to perform Smoke test, will copy in tomcat webroot


Example Playbook
----------------
    
    - hosts: apps
      roles:
      - {name: base-config, tags: base-config} 
      - {name: app-tier, tags: [apps, tomcat]}


