# Learn Terraform - Provision an EKS Cluster


Client Platform used : Ubuntu

Install wget using "sudo apt-get install wget"

# Steps to install Terraform

Platform: Ubuntu

1. Update repository

sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl

2. Add Hashicorp GPG key

curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -

3. Add the official HashiCorp Linux repository.

sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"

4. Update repo and install terraform CLI

sudo apt-get update && sudo apt-get install terraform

5. Verify terraform installation

terraform -help


# Steps to install AWSCLI



curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

Cofigure IAM Details and region specs using command "aws configure" (without quotes)

# Steps to install Kubectl


1. Download latest Release

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

2. Install

sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

3. Validate

kubectl version --client


