1. install ansible
2. git clone 
3. update your env with hadoop nodes.
 example:

###/etc/ansible/hosts
[hadoop]
hadoop1
hadoop2
hadoop3

[hadoop:vars]
ansible_ssh_user=centos
ansible_ssh_private_key_file=/home/centos/.ssh/id_rsa

4. deploy your keys to using nodes
5. run deploy by command:
 
 ansible-playbook main.yml
