# WordPress deployment using Ansible Playbook
Playbook task description:

- Create a Security Group for your intances

- Create an AWS EC2 instance

- As wordpress stores data at the backend in MySQL Database server. Therefore, you need to setup a MySQL server using AWS RDS service using Free Tier.

- Configure the instance with Apache Webserver and php.

- Download WordPress .gz and unarchive.

- Provide the endpoint/connection string to the WordPress application to make it work.

# Prerequisites for this project:
1. AWS Account with Free Tier
2. AWS AMI Access and Secret keys
3. Local machine or EC2 instance with:
   - Python3 and pip3
   - Boto and Boto3
   - Asnible and Ansible-galaxy
   - Ansible-galaxy amazon.aws collection (version 6.10)

How to run the playbook:

ansible-playbook wpansible.yml -i myinventory/hosts.txt 

We use flag -i to specify the hosts.txt file that playbook will use. This code, after creating EC2 instance, will add public_ip and YOUR_KEY name to this file.
