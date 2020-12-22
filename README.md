Setup user account
=========

Setup user account's 

TODO
----
When logging in as user. See information like what domains are installed. A custom message?

Requirements
------------

There are no requirements as of yet


Role Variables
--------------

A complete user with all features would look like this:

```
Users:
  - name: "default"
    env: production
    updatePassword: "always"
    uid: 1501
    mode: 0711
    folderStructure:
      - file: deployments/current
        state: directory
        mode: "0777"
```

The only variable that has to be filled is the `name` var:

```
Users:
  - name: "default"
```

The rest is optional.

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