#  Terraform Aws VPC 

This module creates following resources
* VPC
* IGW
* 2 public subnets in us-east-1a and us-east-1b
* 2 private subnets in us-east-1a and us-east-1b
* 2 database subnets in us-east-1a and us-east-1b
* Public route table and associate public subnets
* Private route table and associate private  subnets
* database route table and associate database subnets
* Elstic ip
* NAT gateway in public sunets
* IGW route is added to public route table
* NAT gateway route to private and database route table
* VPC to default vpc peering
* public route table to default vpc main route table
* default vpc main route table to vpc route table

### INPUTS
* vpc_cidr - (required) user must supply vpc cidr block
* project name - (required) user must supply project name
* environment -(required) user must supply env name
* public_subnet_cidrs -(required) user must supply public subnet cidrs
* private_subnet_cidrs -(required) user must supply private subnet cidrs
* database_subnet_cidrs -(required) user must supply database subnet cidrs
* is_peering_required -(optional) . it is optional

### OUTPUTS
* vpc_id - vpc id is created
* public_subnet_ids - public subnets ids  created 
* private_subnet_ids - private subnets ids  created 
* database_subnet_ids - database subnets ids  created 
* vpc_peering_id - peering connection id is created
