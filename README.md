The development and deploy process will look similar to what is [described here](https://github.com/lachatak/deliverypipeline/blob/master/README.md). 

## Manual cloud env initial setup
You need to do this manually once:

1. Create pub key pair for EC2 using AWS Console. 
2. Download the private key. Do not forget to `chmod 600`.

## Local initial setup 
To be able to run the automation from your machine, you need to do this once: 
1. `sudo pip install boto awsebcli`
1. `./setup.sh`


## Long-term TODO

1. Configure autoscaling 
1. Configure fault tolerance
1. RDS backups
