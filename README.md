# Automate-AWS-with-Ansible
AWS-Ansible  
Connect to AWS services     
AWS CLI configuration and profiles, Ansible Vault, and costing credentials in the Ansible Playbooks.  

Export the AWS secret access key and AWS access key ID:

```
    export AWS_ACCESS_KEY_ID='<YOUR ACCESS_KEY_ID>'  
    export AWS_SECRET_ACCESS_KEY='>YOUR_SECRET_ACCESS_KEY>'
``` 

Avoid hardcoding AWS secrets and keys inside playbooks, store them in an Ansible Vault to encrypt these values before using them:

```
secrets.yml      aws_access_key_id: my-aws-access-key-id  
                 aws_secret_key: my-aws-secret-access-key  
encrypt:     ansible-vault encrypt secrets.yaml  
```

EC2 instance to deploy a web application VPC, a subnet, security groups, and an Internet Gateway attached to the VPC. From AWS_infrastructure: put the code in an Ansible playbook ec2_playbook.yml after run it.  


