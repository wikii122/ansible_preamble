Preamble
=========

Module used to bootstrap server with system user and some basic initialization for further ansible roles.

Requirements
------------

TBD

Role Variables
--------------

- preamble_user - fallback user, by default root, used to setup host when main user was not yet created
- preamble_ssh_key - ssh key to use for service user
- preamble_generate_ssh_key - generate new ssh key for service user on control node (default: false)

Dependencies
------------

By design there should be none - this is the first module to be run on node.

Example Playbook
----------------

    - hosts: all
      roles:
      - wikii122.preamble

License
-------

MIT

Author Information
------------------

Created by Wiktor Ślęczka
