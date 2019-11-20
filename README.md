# chromeos-devops-setup
The following is a set of scripts and commands to setup a chromebook with terraform ansible and visual code studio

Chrome OS has become a DevOps Machine! Here are the steps to install Terraform + Ansible and Visual Code Studio

Here are the Scripts for Terraform:
```
# Install and configure Terraform
# Check for latest release https://releases.hashicorp.com/terraform/
sudo apt-get install wget git unzip gnupg python3 python3-pip -y
sudo apt-get update && sudo apt-get upgrade
sudo wget https://releases.hashicorp.com/terraform/0.12.16/terraform_0.12.16_linux_amd64.zip
sudo unzip terraform_0.12.16_linux_amd64.zip
sudo mv terraform /usr/local/bin/
terraform –version
```

Here are the Commands to Install Ansible:
```
# Install Ansible
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install ansible
ansible --version
```

Here are the Steps to Install Visual Code Studio:
```
sudo pt-get update && sudo apt-get upgrade
sudo wget https://az764295.vo.msecnd.net/stable/f46c4c469d6e6d8c46f268d1553c5dc4b475840f/code_1.27.2-1536736588_amd64.deb
sudo dpkg -i code*-1536736588.deb
# It will fail so need to re-run
sudo apt --fix-broken install
sudo apt-get update
sudo dpkg -i code*-1536736588.deb
```

Enjoy

