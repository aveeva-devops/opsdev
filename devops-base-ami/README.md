# devops

This repo will help to build an immutable AWS AMI with Packer.
Create an identical machine image from a single source

### Create DevOps Base AMI with below softwares

* Docker
* Python
* PIP
* Ansible
* Java
* Jenkins

### Workflow - Image creation
Automation of AMI Creation Using Packer

![Alt text](packer_workflow.PNG?raw=true "Title")

### Use AMI ID - ami-0ff8a91507f77f867. This AMI has below softwares
* Python
* PIP
* Java

### Install ansible (Once you install EC2 using terraform and AMI given)
```
sudo pip install ansible
```
### Install docker
https://serverfault.com/questions/836198/how-to-install-docker-on-aws-ec2-instance-with-ami-ce-ee-update

```
sudo yum install docker -y
sudo service docker start
sudo usermod -a -G docker ec2-user
```

### Install Java 8

```
sudo yum install java-1.8.0
sudo yum remove java-1.7.0-openjdk
```

### Install Jenkins
https://docs.aws.amazon.com/aws-technical-content/latest/jenkins-on-aws/installation.html

```
sudo yum update –y
sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
sudo yum install jenkins -y
sudo service jenkins start
```

