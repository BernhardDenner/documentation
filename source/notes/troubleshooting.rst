===============
Troubleshooting
===============

sudo: unknown uid 42401: who are you?
=====================================

* https://bugs.launchpad.net/kolla-ansible/+bug/1680139

Solution: Stop the ``nscd`` service.
