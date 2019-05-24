This YAML Cloudformation template provisions an AWS Virtual Private Cloud (VPC) into which it creates 2 subnets, each of which are in different Availability Zones. An Internet Gateway is attached to the VPC. Route Tables are created for both subnets - these route traffic via the Internet Gateway. An EC2 Auto Scaling Group (ASG) is set up with a minimum of 2 instances and a maximum of 6 across the 2 subnets. An Application Load Balancer is placed in front of the ASG. The Launch Configuration bootstraps all instances with Apache and copies in the relevant configuration files. 


Prerequisites:

AWS Account with access to CloudFormation

EC2 Key Pair


Getting Started:

Go to Cloudformation and copy in YAML file to create stack.
