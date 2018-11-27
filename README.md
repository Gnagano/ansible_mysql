Ansible role: install mysql server
===

An ansible role to install mysql server and create a default database.

## Requirements

OS: Ubuntu16.04

Pre-installed python (>= 2.0)

## Getting started

```
$ ansible_galaxy install gano2018.ansible_mysql --roles-path <your_roles_directory>
```

and set the role varibles described below.

## Role Varibales

Those role variables are on `defaults/main.yml`.

- mysql_database

This is the variable for the user and the password of the default database.

- mysql_user
- mysql_password

This is the variable for the user and the password of the default database.

- mysql_host

This is the variable for the host for mysql, default value is `localhost`

- mysql_basic_packages

This is the packages required for installation.
