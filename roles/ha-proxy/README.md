Role ha-proxy
=========

This role installs and configures HAPROXY by setting the default log port.

Requirements
------------
playbook settings are in the "tasks\install.yml" directory

For the execution of the playbooks it is necessary to play keys between the servers and perform the role of automation server running ansible.

As the link:
https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2

After this configuration, the internet access of the servers must be guaranteed.

playbook settings are in the "tasks \ install.yml" directory

* ansible-playbook -i hosts main-base.yml


Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults / main.yml, vars / main.yml, and any variables that can / should be set via parameters to the role. Any variables that are read from other roles and / or the global scope (ie. Hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - {role: username.rolename, x: 42}

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).