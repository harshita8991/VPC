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

# Create route tables and attach to subnets 
Route Tables. A route table contains a set of rules, called routes that are used to determine where network 
traffic is directed. Each subnet in your VPC must be associated with a route table; the table controls the routing for the 
subnet. 
One route for Internet gateway, another for Virtual private gateway (R1-IGW and R2-VGW) 
* Route - 0.0.0.0/0 to IGW
* Route - 192.168.0.0/16 to VGW

create route tables ->then add route

![Screenshot 2024-12-01 202158](https://github.com/user-attachments/assets/d69c8fc1-4d62-4775-9175-07b3a10deac6)


![Screenshot 2024-12-01 203132](https://github.com/user-attachments/assets/017e3b80-98f4-438b-9636-798efbae722e)

Attach routing tables to subnets. R1-IGW to S3-Public and S4-Public, public network required to have internet access. 
Attach R2-VGW to S1-Private and S2-Private (No internet become a private subnets)

## create instances

• now we have to create two instnaces    where we have to enable the public     IPv4 .

•then on both instance we have to       downlaod the web server here i have    downlaoded the apache2 server

-- after that i chech that my             instances are working or not .




