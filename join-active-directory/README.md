Role Name
=========

Role to join an active directory

Requirements
------------



Role Variables
--------------

- domain: Active direcory domain to join
- domain_admin_user
- domain_admin_password
- domain_ou_path (ex: "OU=Windows,OU=Servers,DC=domain,DC=local")

Dependencies
------------


Example Playbook
----------------

    - name: join AD
      include_role:
        name: ajoin-active-directory
      vars:
        domain: "domain.local"
		domain_admin_user: admin
		domain_admin_password: "SuperPassw0rd!!"
		domain_ou_path: "OU=Windows,OU=Servers,DC=domain,DC=local"


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
