=============
Configuration
=============

.. toctree::
   :maxdepth: 2

   configuration/cookiecutter
   configuration/synchronisation
   configuration/networks

The basis of an OSISM environment is a configuration repository,
that is divided into individual environments. The structure, the
creation and its contents are explained here.

**Directories**

* ``inventory``: Ansible inventory directory. All host-specific details are managed here.
* ``docs``: Optional directory to manage documents about an environment.
* ``environments``: Directory for managing the individual environments. Each environment has its own subdirectory.

**Environments**

.. toctree::
   :maxdepth: 1

   configuration/environments/manager
   configuration/environments/generic
   configuration/environments/infrastructure
   configuration/environments/openstack
   configuration/environments/ceph
   configuration/environments/monitoring
   configuration/environments/custom
   configuration/update

With the exception of a special environment for the manager, all
environments have the same structure and share the same inventory.

**Files**

* ``configuration.yml``: Default configuration parameters can be overwritten by this file.
* ``images.yml``: This file can be used to overwrite default images.
* ``secrets.yml``: Environment specific secrets can be deposited in this file.
* ``ansible.cfg``: Ansible configuration file.
* ``playbook-*.yml``: Playbook files for Ansible.
* ``environments/ansible.cfg``: Ansible configuration file.
* ``environments/*/ansible.cfg``: Ansible configuration file.
* ``inventory/hosts``
* ``inventory/host_vars/*.yml``
* ``inventory/group_vars/*.yml``
