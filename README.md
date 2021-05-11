# Hadoop_Cluster_Setup_with_Hive_by_Ansible

##WHAT TO DO FOR RUNNING THE SCRIPT->
## For Launching Amazon_instances for namenode,datanode,jobtracker,tasktracker,client you can use instances.yml file and do changes according to your requirements in file var.txt.
## Download above given folder "Hadoop_Cluster_Setup" in your vm and read following steps given below and perform according to it.

1. Change in ansible conf(/etc/ansible/ansible.cfg) file in your vm "inventory='your inventory folder'"
2. Change "roles-path='path of your role'" in ansible conf file that is /etc/ansible/ansible.cfg
3. Change "remote_user='ec2-user'" in ansible conf file that is /etc/ansible/ansible.cfg
4. Change "ansible_private_key='path of your key" in ansible conf file that is /etc/ansible/ansible.cfg
5. Change permission of your private key by run cmd in bash shell "chmod 400 'key name'"
6. For dyanamic inventory run following commands in bash shell
 - export AWS_ACCESS_KEY_ID='access-key-id'
 - export AWS_SECRET_ACCESS_KEY='secret-access-key'
 - export AWS_REGION='region name'
7. 💥💥VERY IMPORTANT POINT FOR SETUP THE CLUSTER
8. ## After reading above instructions for deploying the Hadoop_Cluster_with_Hive setup use "ansible-playbook setupmain.yml" command. 
