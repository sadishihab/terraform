# Infrastructure as Code with Terraform

## Technologies used:

- Terraform, AWS, Docker, Linux, Git, AWS EKS, AWS S3, Jenkins, Java, Maven, Docker Hub,  

## Job 1: Automate AWS Infrastructure
#### Job description:

- Create TF project to automate provisioning AWS Infrastructure and its components, such as: VPC, Subnet, Route Table, Internet Gateway, EC2, Security Group
- Configure TF script to automate deploying Docker container to EC2 instance

## Job 2: Modularize Project
#### Job description:

- Divide Terraform resources into reusable modules

## Job 3: Terraform & AWS EKS
#### Job description:

- Automate provisioning EKS cluster with Terraform

## Job 4: Configure a Shared Remote State
#### Job description:

- Configure Amazon S3 as remote storage for Terraform state

## Job 5: Complete CI/CD with Terraform
#### Job description:

- Integrate provisioning stage into complete CI/CD Pipeline to automate provisioning server instead of deploying to an existing server
- Create SSH Key Pair
- Install Terraform inside Jenkins container
- Add Terraform configuration to application’s git repository
- Adjust Jenkinsfile to add “provision” step to the CI/CD pipeline that provisions EC2 instance
- So the complete CI/CD project has the following configuration:
a. CI step: Build artifact for Java Maven application
b. CI step: Build and push Docker image to Docker Hub
c. CD step: Automatically provision EC2 instance using TF
d. CD step: Deploy new application version on the provisioned EC2 instance with Docker Compose
