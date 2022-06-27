Role Name
=========

Install and setup a windows directory server

Requirements
------------

- A fixed ip address has to be set.
- The hostname should be already set up.
- If not, you can use ansible.windows.win_hostname to set it up before.

Role Variables
--------------

- domain: define windows active directory fomain name, exemple: domain.local
- safemodepw: safe_mode_password

Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Configure AD
      include_role:
        name: active_directory_domain
      vars:
        domain: "domain.local"
        safemodepw: "S@f3Password"


License
-------

BSD

Author Information
------------------


