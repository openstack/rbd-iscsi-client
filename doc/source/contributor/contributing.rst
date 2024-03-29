============================
So You Want to Contribute...
============================

For general information on contributing to OpenStack, please check out the
`contributor guide <https://docs.openstack.org/contributors/>`_ to get started.
It covers all the basics that are common to all OpenStack projects: the
accounts you need, the basics of interacting with our Gerrit review system, how
we communicate as a community, etc.

The rbd-iscsi-client library is maintained by the OpenStack Cinder project.  To
understand our development process and how you can contribute to it, please
look at the Cinder project's general contributor's page:
http://docs.openstack.org/cinder/latest/contributor/contributing.html

Getting Started
---------------

Here are some :doc:`tips for setting up rbd-iscsi-client for local development
<getting-started>`.

Integration Testing
-------------------

The rbd-iscsi-client library is consumed by the Cinder RBD ISCSI driver
(``cinder.volume.drivers.ceph.rbd_iscsi.RBDISCSIDriver``).  The driver,
and hence this library, is tested by the ``cinder-plugin-ceph-iscsi-tempest``
job defined in the ``.zuul.yaml`` file in the Cinder code repository.
