NFS_server_role
=========

Please use this role if you want to make initial setup of NFS server on linux CentOs/RedHat

Requirements
------------

RedHat 6-7

Role Variables
--------------

In a defaults/main you can set the path and name for folder that you want create or set as available for network mounting
and set the host or network that you want to be able to connect to that network share

Example Playbook
----------------

---

- name: install and setup NFS server
  hosts: nfs_server
  become: yes
  
  roles: 
    - "setup_nfs_server"
