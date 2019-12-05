Setup user account
=========

Setup user account's 

TODO
----
When logging in as user. See information like what domains are installed. A custom message?

Requirements
------------

in the inventory file variable like:

    #Define server user name
    Users:
      - name: "default"
        env: production
        updatePassword: "always"
        uid: 1501


Role Variables
--------------

The following varriables are available:
name Required
env default is empty
updatePassword default is to omit
uid default is to omit


Dependencies
------------

None

Example Playbook
----------------

    - name: Setup users
      hosts: all
      roles:
        - ggiinnoo.users

License
-------

BSD

Author Information
------------------

    Creator: Gino Jansen
    Website: www.ginojansen.nl