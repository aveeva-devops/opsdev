# Terraform-aws

This repository contains a [DevOps] projects that builds 
* Scenario 2: VPCwith Public and Private Subnets[scenario_two] from the [AWS documentation][].

## Scenario 2: VPCwith Public and Private Subnets

### Install Terraform on ubuntu 

 ```
git clone https://github.com/chahalpardeep/devops
cd install-terraform ubuntu
sh install_on_ubuntu
 ```

### Usage

terraform.tfvars holds variables which should be overriden with valid ones. First two values are AWS Access key and secret key. Create IAM user and get these values. Last two values are aws_key_pair. Create AWS key-pair from EC2 -> Network and Security -> key-pair.
Change permissions of .pem file to 400, and mention key_name without .pem extension. Execute next two steps to create resources.

### Plan

This will display all the command terraform will execute. This is a dry run.

```
terraform plan -var-file terraform.tfvars
```

### Apply

This will create all the resources mentioned in tf scripts. Ensure to provide valid AMI ID's and your desired aws-region.

```
terraform apply -var-file terraform.tfvars
```

### Destroy

```
terraform destroy -var-file terraform.tfvars
```
