1. create repo for terraform
2.  `terraform init` in the right folder (i.e. our repo that contains our main.tf file)![alt text](image-2.png)
3. `terraform fmt` to standardise our text format and `terraform plan` to generate a plan (note that we haven't saved this)
![alt text](image-3.png)
4. the destructive command `terraform apply` and `yes` to create everything
![alt text](image-4.png)
![alt text](image-5.png)
   - Success:
    ![result of above commands](image-6.png)
1. the destructive command `terraform destroy` and `yes`
![alt text](image-7.png)
![alt text](image-9.png)
   - Success:
    ![alt text](image-10.png) 