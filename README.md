aws-env-list-tool
=================

This is a tool to list aws resources in multiple formats, like ssh-config or /etc/hosts

Features
========
1) List EC2 instances in following formats
    > ssh_config file format
    > /etc/hosts file format
2) Can also update enviroment.
    > Update ssh_config with current running instance list from AWS. (Merge AWS and Non-AWS(on-premise/other) instance groups)
    > Update /etc/hosts with current running instance list from AWS. (Merge AWS and Non-AWS(on-premise/other) instance groups)

To-Do
=====
1) Add auto-complete for bash

Requirements
============
1. python2.6
2. aws credentials saved in ~/.boto file
3. R/W permissions on /etc/hosts and  ~/.ssh_config
4. Non-AWS env files (~/ssh_config_non_aws and ~/hosts_non_aws)  [OPTIONAL]

Usage
=====

1) To list 
    python list_aws_details_for [hosts|ssh]
2) To update
    ./update_my_env
