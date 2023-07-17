# AWS
# Amazon Web Service
# AWS CLI
aws ec2 run-instances --image-id ami-053b0d53c279acc90 --instance-type t2.micro --key-name aws-login --subnet-id subnet-0ebab1769cc5fbf98 --security-group-ids sg-01b32af20c096fef4 --tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=MyInstance}]'
