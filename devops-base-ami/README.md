# devops

### This repository contains a [Terraform-aws] projects that builds 
* Terraform-aws - Scenario 2: VPCwith Public and Private Subnets[scenario_two] from the [AWS documentation].
* Refer AWS Documentation to understand VPC scenario 2 - https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Scenario2.html

### Create DevOps Base AMI with below softwares
* Docker
* Python
* PIP
* Conda
* Ansible
* Java
* Jenkins

### Use AMI ID - ami-0ff8a91507f77f867. This AMI has below softwares
* Python
* PIP
* Java

### Install ansible (Once you install EC2 using terraform and AMI given)
```
sudo pip install ansible
```
### Install docker
* https://serverfault.com/questions/836198/how-to-install-docker-on-aws-ec2-instance-with-ami-ce-ee-update

```
sudo yum install docker -y
sudo service docker start
sudo usermod -a -G docker ec2-user
```
### Install Jenkins
* https://docs.aws.amazon.com/aws-technical-content/latest/jenkins-on-aws/installation.html

```
sudo yum update –y
sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
sudo yum install jenkins -y
sudo service jenkins start
```

