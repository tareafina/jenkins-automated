**Under this project we will recreate a development environment with the following technologies**

* Ansible
* Vagrant
* Powershell/Bash
* Docker
* Cloud Provider (GCP/AWS/Azure)
* Jenkins
* Terraform
* Webserver (Nginx/Apache)
* OS (Ubuntu/CentOS)

The main idea of this project is generate some automated infrastructure from scratch as below and save the outputs to provide all the information at the end of the project (such as endpoints, instances, etc).

**We will follow the below path (in general terms) to get this project up:**

* Validate dependencies
* Create local VMs with Vagrant
* Configure the VMs with Ansible Playbooks
* Run Jenkins
* Create Terraform templates
* Create on Jenkins the Jobs/Pipeline to deploy the Terraform templates
* Deploy the infrastructure to the cloud provider
* Run a dockerized webserver
* Provide the outputs

The main key of the project is improve the scripting skills to, so we will try to automatize all the possibles tasks.

**We are doing this Initials test with the following software Versions**

* Vagrant: 2.2.7
* Ubuntu: 18.04 (WSL)
* Ansible: 2.5.1
* VirtualBox: 6.1

**To execute this environment download the repository**

`git clone https://github.com/tareafina/jenkins-automated`

**Then inside of the directory**

`vagrant up`

**If is necessary add the following variables**

`export PATH=$PATH:'/c/Program Files/Oracle/VirtualBox'`
`export VAGRANT_WSL_ENABLE_WINDOWS_ACCESS="1"`
