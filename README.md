# IDM-Ansible
Playbook examples for IdM tasks

These examples are using Ansible Automation platform and expect the following variables

Your vars will vary and if not using Ansible Automation platform the follwing vars will live in the inventory file
```
# server vars
ipaadmin_admin: 'admin'
ipadm_adm: 'Directory Mananager'
ipaadmin_password: 'yourpassword for the admin account'
ipadm_password: 'your password for the Directory Server account'
ipaserver_domain: your.domain
ipaserver_realm: YOUR.REALM
ipaserver_setup_dns: true
ipaserver_install_packages: yes
ipaserver_setup_firewalld: no   
ipaserver_mem_check: no
ipaserver_no_host_dns: true
ipaserver_allow_zone_overlap: true
ipaserver_no_forwarders: true

# replica vars
ipaserver_domain: your.domain
ipaserver_realm: YOUR.REALM
ipareplica_setup_ca: yes
ipaserver_ignore_topology_disconnect: true
ipaservers: ipaserver-demo.server.lab
ipaclient_servers: ipaserver-demo.server.lab
ipaserver_hostname: ipaserver-demo.server.lab
ipareplica_skip_conncheck: no
ipaclient_force_join: true

# client vars
ipaadmin_principal: admin
ipaclient_domain: your.domain
ipaclient_configure_dns_resolver: no
ipaclient_servers: ipaserver-demo.server.lab
ipaserver_hostname: ipaserver-demo.server.lab

# topology
right and left server must be set

```
