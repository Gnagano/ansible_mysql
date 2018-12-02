Ansible role: install mysql server
===

### Overviews

This roles build mysql server environment automatically.
The details what the roles do are

- install required packages
- install mysql server
- create new database and new user
- create root user if you need

## Requirements

OS: Ubuntu16.04

Pre-installed python (>= 2.0)

## Getting started

```
$ ansible_galaxy install gano2018.ansible_mysql --roles-path <your_roles_directory>
```

and set the role varibles described below.

## Usage

Copy `defaults/main.yml.default` as `defaults/main.yml` and edit the role variables in main.yml.
The details of role variables are described below.

## Role Varibales you need to edit

Those role variables are on `defaults/main.yml`.


#### create_root

If the value is `yes`, ansible craete root user. The default value is `no`

#### root_user_name

Name of root. You need to name execpt `root`. If the value of this variable is `root`, nothing happen.

#### root_user_password
#### root_user_host

As the name of the variables, please set the root password and host.

#### mysql_database
#### mysql_user
#### mysql_password
#### mysql_host
#### mysql_test_database
#### mysql_test_user
#### mysql_test_password
#### mysql_test_host

You need to create two database, one is project's main database and the other is the database for test.
Please specify the database name, access user name, password and host on these fields.
