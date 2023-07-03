# WordPress deployment using Ansible Playbook
Prerequisites for this project:
1. AWS Account with free tier
2. AWS AMI Access and Secret keys
3. Local machine or EC2 instance with:
   - Python3 and pip3
   - Boto and Boto3
   - Asnible and Ansible-galaxy
   - Ansible-galaxy amazon.aws collection (version 6.10)

How to run the playbook:
ansible-playbook wpansible.yml -i myinventory/hosts.txt 
We use flag -i to specify the hosts.txt file that playbook will use. This code, after creating EC2 instance, will add public_ip and YOUR_KEY name to this file.
