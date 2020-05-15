Role install-helm
=========

This role is installed on the monitoring stack with prometeus operator.

Requirements
------------

playbook settings are in the "tasks\install.yml" directory
For its installation it is necessary that the cluster is in the air its execution will be done through the playbook main-monititools.yml, with the syntax:

ansible-playbook -i hosts main-monititools.yml

Role Variables
--------------

helm_url: https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3

Dependencies
------------
This role depends on the cluster in general.


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