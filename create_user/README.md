# ansible-create-users

Create on each server (file hosts) users from the list (file users.yml).

![ansible-create-users](https://bytebucket.org/grydev/ansible/raw/c963f117c21f5786c3b1a308fd37e20c7da83a4e/user_mgmt/ansible-create-users.jpg?token=ea6bdac2f2bc1b1afaa6967b3b6c37effa244574)

User Settings
------------

- Shell = /bin/bash
- Add the public key in pub_keys dir (username.pub)
- In users.yml specify that user should have the right to sudo or not

Distros tested
------------

Currently, this is only tested on Ubuntu 14.04 as a client and server machine. It should theoretically work on older versions of Ubuntu or Debian based systems.

Usage
------------
- install ansible
- create keys
- configure client server authorized_keys
- upload repository and change
- run command

```
ansible-playbook -i hosts create_users.yml
```
