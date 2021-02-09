:orphan:

.. highlight:: shell

.. _getting-started:

Get Started!
============

Ready to contribute?

Local setup
-----------

Here's how to set up ``rbd-iscsi-client`` for local development.

1. Clone the ``rbd-iscsi-client`` git repository::

    $ git clone https://opendev.org/openstack/rbd-iscsi-client.git

2. Install your local copy into a virtualenv. Assuming you have
   virtualenvwrapper installed, this is how you set up your repo for local
   development::

    $ mkvirtualenv rbd-iscsi-client
    $ cd rbd-iscsi-client/
    $ python setup.py develop

3. Create a branch for local development::

    $ git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

4. When you're done making changes, check that your changes pass flake8 and the
   tests, including testing other Python versions with tox::

    $ tox -e pep8
    $ tox

   To get flake8 and tox, just pip install them into your virtualenv.

5. Commit your changes and push them to the opendev gerrit.  (Please follow
   the OpenStack standard for commit messages.  If you haven't already, you'll
   need to install the ``git-review`` package from your operating system
   distro first)::

    $ git add .
    $ git commit
    $ git review

Submission Guidelines
---------------------

Before you submit a patch, check that it meets these guidelines:

1. The patch should include tests.
2. If the patch adds functionality, the docs should be updated. Put
   your new functionality into a function with a docstring and add a
   release note to your patch.
3. The patch should work for at least Python 3.6 and 3.8.

Tips
----

To run a subset of tests::


    $ tox -epy38 tests.test_rbd_iscsi_client
