# AnsibleforAWS
## Create a Key pair and Launch a EC2 instance in Aws account using Ansible

## Ansible for Aws 


1. Authentication

First, create an IAM user
Put the access key and secret key in .bashrc file 


vim .bashrc

source .bashrc

After that authentication is done 
Then logout and login

mkdir aws
cd aws
vim test-aws.yml
ansible-playbook test-aws.yml

At the time of running this playbook, we can get the error message because 
some libraries to access different resources like AWS.
For that, it has a module called boto or
boto three, which Ansible is not able to find.
And we need to install this module.
It's a Python module.
And we are going to use the
command Pip to install this module.
The command will be basically pip install boto three.
But it's not going to work because we do not have Pip.
First, we have to install app and install Python Pip.

Sudo apt install python -pip
Pip install boto3
Ansible-playbook test-aws.yml

You are successfully launched a EC2 instance using Ansible
