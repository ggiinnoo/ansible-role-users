Setup user account
=========

Used to setup user accounts on the server

TODO
----
When logging in as user. See information like what domains are installed. A custom message?
using the .bash_profile to set the env like production dev etc

Requirements
------------

in the inventory file variable like:

    #Define server user name
    Users:
      - name: "default"
        updatePassword: "always"
        uid: 1501


Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

    - name: Setup users
      hosts: groupWeb
      roles:
        - users

License
-------

BSD

Author Information
------------------

    Creator: Gino Jansen
    Website: www.ginojansen.nl