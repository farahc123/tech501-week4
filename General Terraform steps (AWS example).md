# General steps when using Terraform

- [General steps when using Terraform](#general-steps-when-using-terraform)
  - [Steps (creating an EC2 instance as an example)](#steps-creating-an-ec2-instance-as-an-example)
  - [Helpful links](#helpful-links)

## Steps (creating an EC2 instance as an example)

1. create repo for terraform
2.  `terraform init` in the right folder (i.e. our repo that contains our main.tf file)![alt text](image-2.png)
3.  `terraform validate` to validate the syntax of our .tf files
4. `terraform fmt` to standardise our text format and `terraform plan` to generate a plan (note that we haven't saved this)
![alt text](image-3.png)
1. the destructive command `terraform apply` and `yes` to create everything
![alt text](image-4.png)
![alt text](image-5.png)
   - Success:
    ![result of above commands](image-6.png)
1. the destructive command `terraform destroy` and `yes`
![alt text](image-7.png)
![alt text](image-9.png)
   - Success:
    ![alt text](image-10.png) 

## Helpful links
- [Terraform official documentation](http://developer.hashicorp.com/terraform)
- [Windows tool for creating Azure instances using Linux](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-terraform?tabs=azure-cli); note that HC documentation is preferable because they updated their syntax often and this isn't always reflected in third-party resources
- [Template for creating EC2 instances in Terraform](https://github.com/terraform-aws-modules/terraform-aws-ec2-instance)
- [Template for creating AWS security groups in Terraform](https://github.com/terraform-aws-modules/terraform-aws-security-group)
- [Template for creating AWS VPCS i.e. virtual networks in Terraform](https://github.com/terraform-aws-modules/terraform-aws-vpc)
- [More templates for creating AWS resources in modular format in Terraform](https://github.com/terraform-aws-modules)
