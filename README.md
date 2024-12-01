# VPC
A virtual private cloud (VPC) is a virtual network dedicated to your AWS account. It is logically isolated from
other virtual networks in the AWS Cloud. You can launch your AWS resources, such as Amazon EC2 instances, into your
VPC.

![image](https://github.com/user-attachments/assets/68942c35-be00-4be2-8234-d282f5941caf)

# Create VPC
for creating a VPC , follow the following steps:
go to AWS Console ,then click Services ,then go to Networking & Content Delivery , click on VPC , click on Your VPCs.
after these steps on click on create VPC.

![Screenshot 2024-12-01 184945](https://github.com/user-attachments/assets/1dd28f0d-995e-4fa9-a5a8-58195eb430b3)

 # Create subnets

![Screenshot 2024-12-01 190639](https://github.com/user-attachments/assets/d7537bd5-63b4-4696-a6e4-f5f60b56bd39)

# Create Internet gateway and attach to VPC 
Internet Gateways. An internet gateway is a horizontally scaled, redundant, and highly available VPC component 
that allows communication between instances in your VPC and the internet. It therefore imposes no availability risks or 
bandwidth constraints on your network traffic.

create a gateway then attach it to your VPC ,

![Screenshot 2024-12-01 191305](https://github.com/user-attachments/assets/50158fb6-5dbc-4245-8881-373d021b6775)

# Create Virtual Private Gateway and Attach to VPC 
It can be a physical or software appliance. The anchor on the AWS side of the VPN connection is called a virtual 
private gateway. The following diagram shows your network, the customer gateway, the VPN connection that goes to 
the virtual private gateway, and the VPC.
create a VPGW-> actions -> attach to VPC

![Screenshot 2024-12-01 192031](https://github.com/user-attachments/assets/974f38e1-fd76-4c59-bd90-fa838f4a156c)

