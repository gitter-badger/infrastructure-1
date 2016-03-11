The development and deploy process will look similar to what is [described here](https://github.com/lachatak/deliverypipeline/blob/master/README.md). 

You will need to install [Ansible](https://www.ansible.com/) to be able to run the code in the repo.

Also, you should have [AWS Access Key](http://docs.aws.amazon.com/general/latest/gr/getting-aws-sec-creds.html) for your IAM user available in your local environment (defined as `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` env variables).

## Manual cloud env initial setup

[![Join the chat at https://gitter.im/WorldBrain/infrastructure](https://badges.gitter.im/WorldBrain/infrastructure.svg)](https://gitter.im/WorldBrain/infrastructure?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
You need to do this manually once:

1. Create pub key pair for EC2 using AWS Console. 
2. Download the private key. Do not forget to `chmod 600`.

This is necessary for Ansible to being able to connect EC2 servers behind Beanstalk.

## Local initial setup 
To be able to run the automation from your machine, you need to do this once: 

1. `sudo pip install boto awsebcli`
1. `./setup.sh`


## Long-term TODO

1. Configure autoscaling 
1. Configure fault tolerance
1. RDS backups
