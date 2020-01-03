Role Name
=========

.List of Roles
[%header,cols=2*]
|===
| Directory | Purpose
| app-tier | Install application server role
| db-tier  | Install postgressql server for database role
| lb-tier  | Install HA proxy role
| base-config | Setup yum repo and base packages role
| setup-workstation | Setup workstation, create network, ssh keypair, security group etc. role 
| osp-servers | Provision OSP Instances role
| osp-instance-delete | Delete OSP Instances role
| osp-facts | Genrate in-memory inventory for OSP instances role
| config-tower | Role to configure ansible tower job templates and workflow
|===


