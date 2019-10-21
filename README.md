# Using CloudFormation VPC with private and public subnets

A VPC is a virtual network inside AWS where you can isolate your setup using private IP addresses. A VPC consists of several subnets.
A public subnet has a direct route to the Internet. As long as your EC2 instances have an public IP they can communicate (in and out) with the Internet. A private subnet does not have a route to the Internet. Instances in private subnets can not be accessed from the public Internet. 
If you want to access the Internet from a private subnet you need to create a NAT gateway/instance. 
You can deploy a bastion host/instance to reduce the attack surface of internal applications.

## Infrastructure Architecture
![VPC-Template](https://user-images.githubusercontent.com/15983893/66629611-edd7e080-ec1f-11e9-849b-f60e144a05a2.png)

 
## Parameters

![VPC-Parametr-ParentStack](https://user-images.githubusercontent.com/15983893/66628911-d5ff5d00-ec1d-11e9-95cf-a0b3f59c0107.PNG)



