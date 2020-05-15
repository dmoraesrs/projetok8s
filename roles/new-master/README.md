Role new-master
=========

This role should be used to add a new server to the cluster with the role of Worker

Requirements
------------
playbook settings are in the "tasks\install.yml" directory
For the execution of the playbooks it is necessary to play keys between the servers and perform the role of automation server running ansible.

As the link:
https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2

After this configuration, the internet access of the servers must be guaranteed.

* ansible-playbook -i hosts main-base.yml
* ansible-playbook -i hosts main-Install-k8s.yml

After running the playbooks above, the server that will be the new worker member must be placed in the hosts file in the "[k8s-master-new]" session. After this configuration run the playbook.

* ansible-playbook -i hosts main-master.yml

After completion, it must be removed from the session and added to the session "[k8s-master]"


Role Variables
--------------

[k8s-workers: vars]
K8S_MASTER_NODE_IP = haproxy
K8S_API_SECURE_PORT = 6443


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).