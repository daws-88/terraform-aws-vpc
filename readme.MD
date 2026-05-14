# VPC Module
* This module is devloped for joindevops company. Projects inside joindevops should follow this module

### Inputs
* project(required) - Users must specify project name
* environment (required) - Users should specify their  environment
* cidr_block (optional) - Users can provide their CIDR block. Default is 10.0.0.0/16

### Outputs
* vpc_id - Exports VPC ID created