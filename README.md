# Week 4

- [Intro to Terraform](<Terraform intro.md>)
- [General steps for using Terraform](<General Terraform steps.md>)
- [Using variables in Terraform](<Terraform variables.md>)
- [Deploying our 2-tier app on Azure using Terraform](<Azure and Terraform 2-tier deployment/Azure and Terraform VN and VMs steps steps.md>)
- [Code for deploying an EC2 instance using Terraform](https://github.com/farahc123/tech501-terraform/tree/main/create-ec2-instance)


## Workflow for creating a new local repo and syncing it to a new Github repo

-   create local repo folder
-   `git init` — initialises the repo
-   create repo on GitHub
-   `git commit -m "first commit"` 
- `git branch -M main` — renames current branch (always master by default) to *main*
-   `git remote add origin <link to github repo e.g. <https://github.com/farahc123/tech501-week2.git>>` — specifies the remote repo (e.g. a github repo, which is the *origin*) so you can create, view, and delete connections to it
-   ` git push -u origin <branch name e.g. main>` — does the first sync of the files and commit history to the previously added remote repo
