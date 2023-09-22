conditions
variables
data types
functions
loops

count and count index
outputs
data sources
locals

vpc and vpc peering

VPC
-------------
VPC
IGW and associate with VPC
Public, private and DB subnets HA in 2 AZ
public private and DB RT
we are adding routes
NAT gateway --> as a route to private and DB subnets
	egress traffic is always through NAT, ingress is not allowed
assoications of RT and subnets

VPC peering
----------
Default VPC
requestor --> Default VPC
acceptor --> roboshop VPC
default route table
-------------------
you should have a road to roboshop VPC, it means 

destination is roboshop CIDR, road is peering connection

roboshop route tables
-------------------
you should have road to default VPC, it means
des' is default VPC CIDR, road is peering connection

create EC2, SG is allow-all from your IP

terraform has access to the current folder, it cant go to another folder/projects and bring the values

vpc
vpn
mongodb

person-1 wants help, but his SG not allowing others
person-2 is ready to help

person-1 should add IP address of person 2 to his VPN

either add CIDR or add security group attached to EC2 instance

2 VPN --> MongoDB

source: VPN
destination: mongodb

in mongodb SG, if I add the SG of VPN instance, I am allowing traffic only from the instance connected with SG of VPN

2 VPN --> VPN SG

Mongodb --> VPN SG as SG rule

MongoDB allow connections from the instances that have sg group as sg-004936dae035e599b