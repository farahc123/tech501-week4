# Steps

- [Steps](#steps)
  - [Setting up Azure CLI](#setting-up-azure-cli)
  - [Creating the 2-subnet virtual network with their NSGs](#creating-the-2-subnet-virtual-network-with-their-nsgs)
    - [Results](#results)
  - [Creating the app VM](#creating-the-app-vm)
    - [Results](#results-1)
  - [Creating the DB VM](#creating-the-db-vm)
    - [Results](#results-2)


## Setting up Azure CLI

1. download azure CLI on powershell with `winget install --exact --id Microsoft.AzureCLI`
2. open a new git bash window
3. run `az login` and choose my Sparta account
4. press Enter (i.e. don't enter a subscription ID)

## Creating the 2-subnet virtual network with their NSGs

- Different cloud providers use different syntax, so for this task I had to research the Azure VN-related syntax in Terraform
- I created variables in a *variable.tf* file that has been gitignored to ensure the security of sensitive information 
- [Terraform provisioning code here](https://github.com/farahc123/tech501-terraform/blob/main/create-2-subnet-vnet/main.tf)

### Results

- Azure 2-subnet VN created with Terraform
![alt text](image.png)

## Creating the app VM

- Different cloud providers use different syntax, so for this task I had to research the Azure VM-related syntax in Terraform
- I created variables in a *variable.tf* file that has been gitignored to ensure the security of sensitive information 
- [Terraform provisioning code here](https://github.com/farahc123/tech501-terraform/blob/main/create-azure-app-vm/main.tf)


### Results

- An app VM created with Terraform
![alt text](image-1.png)

- Proof that my app works on the above VM
![alt text](image-2.png)

## Creating the DB VM

- I used similar syntax to the app VM, but I removed the public IP assignment to replicate the security we set up manually on Azure
- I created variables in a *variable.tf* file that has been gitignored to ensure the security of sensitive information 
- [Terraform provisioning code here](https://github.com/farahc123/tech501-terraform/blob/main/create-db-vm/main.tf)

### Results

- A DB VM created with Terraform (to be added)

- Proof of my posts page working (to be added)