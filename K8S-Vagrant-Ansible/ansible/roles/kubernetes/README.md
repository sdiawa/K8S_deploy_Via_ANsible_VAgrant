Role Name
=========

A brief description of the role goes here.

Requirements
------------
Installer : Vagrant, Ansible

Installer ces deux plugins 
vagrant plugin install vagrant-faster
vagrant plugin install vagrant-cachier
pour ne pas avoir  l'erreur : "* Unknown configuration section 'cache'." au moment du vagrant up,

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

COMMENCER PAR LA CONFIGURATION DU MASTER1 kubm1

vagrant up kubm1 dans /vagrant

ansible -i inventory.yml all, -m ping -u vagrant dans /ansible/

ansible-playbook -i inventory.yml -u vagrant -l kubm1 playbook.yml dans /ansible/

* Apres deploiement sur KUBM1

vagrant ssh kubm1  
=> pour verfifier installation

dpkg -l | grep kubelet ou dpkg -l | grep kube





