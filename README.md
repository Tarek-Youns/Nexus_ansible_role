Role Name : install
=========

Role to install Nexus

Requirements
------------

Install OpenJDK 1.8
Install wget

Role Variables
--------------
Dirctory_app
downloaded_file
Archive
Old_name
New_Name
configration_path
Service_file

Example Playbook
----------------
   - name: install Nexus


    - hosts: servers #your hosts
      remote_user: tarek  # choice user to run the commands in the remote machine 
      become: true  # to give sudo to the user 
      roles:
         - install   #role name 

finally use this command to run the role
ansible-playbook playbook.yml -i inventory --ask-become-pass


BSD
Tarek youns
------------------

