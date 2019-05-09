# Ansible Role: POSTFIX-SERVER
=========

Prepare an PostFix-server on RedHat/CentOS or Debian/Ubuntu

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, along with default values (see `default/main.yml`):

A list of variables which will be placed in the `/etc/postfix/main.cf` configuration file. 


    myhostname : server.example.com
    mydomain : example.com
    inet_interfaces : all
    inet_protocols : ipv4
    mydestination : $myhostname, localhost.$mydomain,...
    mynetworks : 192.168.33.0/24

Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: zk.postfix }

License
-------

GPLv3

Author Information
------------------

This role was create in 2019 by [Zakaria Kebairia] 
