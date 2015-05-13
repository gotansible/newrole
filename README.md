newrole
=========

[![Build Status](https://travis-ci.org/gotansible/newrole.svg)](https://travis-ci.org/gotansible/newrole)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-runit-blue.svg?style=flat)](https://galaxy.ansible.com/list#/roles/3780)

Creates a scaffolding for a new ansible role. It was created because the one that comes with Ansible (ansible-galaxy) leaves something to be desired.

Requirements
------------

*nix OS - Debian, Ubuntu, CentOS, RedHat, Amazon Linux, etc..		

Role Variables
--------------

newrole_name: the_name_of_the_new_role
newrole_dest: /the/path/to/create/the/new/role

Dependencies
------------

None

Setup
----------------

**Step 1**
Get the newrole folder onto your computer.

```bash
ansible-galaxy install gotansible.newrole 
```

or

```bash
ansible-galaxy install gotansible.newrole -p ~/src/pick_a_folder_to_put_it_in
```

**Step 2**
Make it easy to run newrole.

```bash
echo "alias newrole='/etc/ansible/roles/newrole/newrole'" > ~/.profile
source ~/.profile
```
or (if you picked a specific folder)

```bash
echo "alias newrole='/path/to/the/folder/in/step/1/newrole/newrole'" > ~/.profile
source ~/.profile
```

**Step 3**
Runit

newrole my_groovy_new_role_name

License
-------

MIT

Author Information
------------------

Created by Franklin Wise in Santa Monica, CA.

