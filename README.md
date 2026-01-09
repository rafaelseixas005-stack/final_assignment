Note: this repo stores scripts for students to play with (several errors can be found in the scripts, i.e., credentials)

*Final assignment*

team:  max group of 3 people

Delivery date: 9 January 2026

Exercise 1
1. Fork this repository
2. in the new repositry, make sure that:
   a) a proper index.html file is served by NGINX
   b) make sure passwords are not shown in the Terraform and Ansbile files (they are not visible in the repository)
  

Exercise 2:
1. Create a new repository
2. Create a Linux machine in Azure that will play a DHCP role (test the configurarion)
3. use Terraform and Ansible (zero manual configuration)
4. make sure that no passwords are stored in scripts
5. delivery the code in a github repo

TIP: https://techcommunity.microsoft.com/blog/azurenetworkingblog/custom-dhcp-support-in-azure/4089674

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

#1 To use the repo you should:
      copy the repo and create an azure account 

#2 On terminal put the following commands:
      
	sudo apt update 
	az login (login into the account)
	sudo apt install ansible 
	sudo apt install terraform
	sudo apt install openssh-client -y

#### (if you want you can change the azure region just go to the main.tf file and change in 1. were says "spaincentral") ####

#3 On the repo past execute:
      
	terraform init
	terraform plan
	terraform apply 

#4 Go to the azure: 
      resource groups -> my-terraform-rg -> my-ubuntu-vm -> connect -> edit settings -> reset ssh private key -> run the command

#5 Change the "ssh -i <private-key-file-path>" with the path of the dowloaded key

#6 Run your cloud Vm without problems 
