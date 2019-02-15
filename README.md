# Ansible_EC2_Docker_Nignx
Ansible_EC2_Docker_Nignx_Autimation

Ansible-ec2-docker-Nginx-deployment
Deploy nginx via docker on AWS ec2 by Ansible Automation.

Prerequisites:

Pythonv2.7
Ansible
Python Boto
Git

Plan


![image of Plan_AnsibleEC2DockerNginxx](https://github.com/KaneWen/Ansible_EC2_Docker_Nignx/blob/master/Plan_AnsibleEC2DockerNginxx.png)
 
Figure 1  : Ansible-ec2-docker-Nginx-deployment

The plan of the module is deploying via a Personal Computer (PC), the Ansible is install in the Virtual Machine CentOS7 Operating System (OS). Ansible Play-book to Create Security Group (SG), Virtual Private Cloud(VPC) ,install Docker and Nginx Docker Image.

The steps:
1 Install  Ansible on VM CentOS7
yum install epel-release
yum -y install ansible
ansible –version        # Check version of Ansible, result : ansible 2.7.6
ssh-keygen               # creat public/private rsa keypair
##Install boto
yum -y install python-pip
 pip install -U boto
pip install boto boto3

2 AWS 
Create Group and User and Security Credential on IAM console.
Create key pair on EC2 console.

3 Security Group 
Create Security Group and EC2 instance

Ansible_create_sg_instance.yml

Modify ports of the security  group

Ansible_modify_sg_ports.yml


4 VPC  # To be edited

5 Docker  # To be edited

6 Nginx Docker image # To be edited
