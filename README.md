----------------------ansible----------------
What is Ansible?

Ansible is an open source, command-line IT automation software application written in Python. It can configure systems, deploy software, and orchestrate advanced workflows to support application deployment, system updates, and more. Ansible's main strengths are simplicity and ease of use.

#How Ansible works?

In Ansible, there are two categories of computers: the control node and managed nodes. The control node is a computer that runs Ansible. There must be at least one control node, although a backup control node may also exist. A managed node is any device being managed by the control node.
sudo yum update -y

sudo yum install ansible -y

log in to main server (Ansible)
=================================
# Connection process (SSH)
===================================
generate keys 
ssh-keygen --copy public ip(id_rsa.pub) and paste it into target server path .ssh/authorizedkeys

so now Ansible server able to ping target server 

======================================
# Inventory File Process
=======================================
What is Inventory File?

Inventory defines the managed nodes you automate, with groups so you can run automation tasks on multiple hosts at the same time
Create our own inventory file vi inventory and add target private ips

or 

We can add target private ips into defualt path of inventory fiel

path--- vi /etc/ansible/hosts
