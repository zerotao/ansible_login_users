Role Name
=========

login_users

Description
-----------

Rule to create normal users, add ssh keys and manage sudo permissions

Requirements
------------

Ansible 1.2

Role Variables
--------------

    users:
      <username>:
        full_name: <String>
        groups: <String List>
        ssh_key: <Path>
        shell: <Path>
        sudo: <Boolean>

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: login_users
           users:
             'jdoe':
                full_name: John Doe
                groups: admin
                ssh_key: user_keys/jdoe.pub
                shell: /bin/zsh
                sudo: True

License
-------

BSD

