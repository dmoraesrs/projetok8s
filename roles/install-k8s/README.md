Role install-k8s
=========

In this role we have the procedure for installing k8s dependencies and packages:

Requirements
------------


playbook settings are in the "tasks\install.yml" directory
    - docker
    - kubelet
    - kubeadm
    - kubectl

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults / main.yml, vars / main.yml, and any variables that can / should be set via parameters to the role. Any variables that are read from other roles and / or the global scope (ie. Hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

In this install.yml file we have the procedure for installing dependencies and packages for k8s:
    - docker
    - kubelet
    - kubeadm
    - kubectl

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