# Ansible-Hadoop-ClientNode-Role

An Ansible Role to Configure and setup [Hadoop](https://hadoop.apache.org/) Client Node.

Requirements
------------
This role is dependent upon `shubhambhardwaj007.ansible_hadoop_software_installation_role`.
For a full usage example with the `shubhambhardwaj007.ansible_hadoop_software_installation_role` role, see the Example Playbook later in this README.

Role Variables
--------------
Available variables are listed below, along with default values (see vars/main.yml):
> Name_Node_Hdfs_Port: "9001"
> Job_Tracker_Mapreduce_Port: "9002"

The `Name_Node_Hdfs_Port` should be similar to exposed port by Hadoop Master Node.
The `Job_Tracker_Mapreduce_Port` should be similar to exposed port by Hadoop Job Tracker Node.

Dependencies
------------
None

Example Playbook
----------------
> - hosts: client_node
>   roles:
>     - shubhambhardwaj007.ansible_hadoop_software_installation_role
>     - shubhambhardwaj007.ansible_hadoop_clientNode_role
License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
