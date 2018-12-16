zoidy_troglodyte
================

An Ansible role to mildly lockdown Ubuntu/Mint.

Requirements
------------

A box running Ubuntu or similar (preferably Linux Mint MATE).

Example Playbook
----------------

It's simple to run the role from a playbook::

  - hosts: servers
    roles:
       - role: zoidy_troglodyte

This role needs to become ``root`` to install packages,
so add ``-K`` to be prompted for the password.::

  ansible-playbook path/to/site.yml -K

If you want to restrict what's installed to a specific group, use tags, e.g.,::

  ansible-playbook path/to/site.yml -K --tags disable-password-auth

License
-------

`GPLv3 <LICENSE>`__

