# lampstack
1. Install Ansible using DNF
 dnf install epel-release -y
 dnf install ansible -y
 ansible --version
2. Setup SSH Passwordless Authentication
 ssh-keygen -t rsa
 ssh-copy-id root@192.168.10.138
 ssh root@192.168.10.138
3. Create Ansible Inventory
 [centos]
 node1 ansible_host=192.168.10.138 ansible_user=root
 ansible --list-hosts all
5. Create Ansible Playbook to Install LAMP Server on Remote Nodes
6. configuring playbook
