# Anisble Role: snowsql
Ansible role to install and configure snowsql in any given instance, user and folder

## Requirements
None.

##Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    user: ec2-user
The user under which snowsql will be installed and configured.

    target_folder: /home/{{user}}
No need to pass any value for the target_folder variable as this is target home path of the user against which the installation in planned. This is explained here as a reference

    db_account_name: snowflake_account_name 
This account name of the Snowflake intented to be configured for the client

    db_region: snowflake_region
This is the region of the snowflake database

    db_user_name: snowflake_username
This is the user name to be used for snowflake connection

    db_password: snowflake_password
This is the password credential for snowflake database

## Dependencies
None.

## Example Playbook
  - hosts: localhost
    roles:
      - { role: gvnirmalaa.snowsql }
# License
MIT / BSD

## Author Information
This role was created in 2019 by Nirmala, author of ansible-role-snowsql.
