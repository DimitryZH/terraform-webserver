# Provisioning an Apache Web Server with Terraform on AWS via GitHub Integration with Terraform Cloud

## Overview:
This project demonstrates the deployment of an Apache web server using Terraform on the AWS cloud infrastructure. The Terraform code for this deployment is stored in a GitHub repository, which is connected to a Terraform Cloud project. The workflow involves initiating the creation of the web server in Terraform Cloud, performing a plan, and applying the configuration. The Terraform code is then fetched from GitHub and utilized to provision the infrastructure on AWS.

## Process:
1. **Setup in Terraform Cloud**: The project begins by setting up a Terraform Cloud project where the infrastructure will be managed. This involves linking the project to the appropriate version control system (GitHub) and configuring necessary variables (AWS access key and secret key).

2. **Terraform Plan and Apply**: Once the project is set up, the user initiates the provisioning process by creating a Terraform plan. This plan is reviewed to ensure accuracy before proceeding. Upon approval, the configuration is applied, and the infrastructure resources are provisioned on AWS.

3. **GitHub Integration**: The Terraform configuration code is stored in this GitHub repository, allowing for version control and collaboration. The Terraform Cloud project is connected to this GitHub repository, enabling seamless integration and automatic updates when changes are made to the codebase.

4. **Provisioning on AWS**: After the Terraform plan is applied, the configuration is fetched from GitHub and utilized to provision the specified resources on AWS. This includes launching an EC2 instance with an Apache web server, associating it with an Elastic IP, and configuring security groups to allow HTTP traffic.

## Results:
The screenshots below showcase the successful deployment:

1. **Terraform Run (Apply Finished)**:
   
   ![Terraform Apply Finished](https://github.com/DimitryZH/terraform-webserver/assets/146372946/845d2398-3093-4d9f-86ef-32fb4fa7aa42)

3. **AWS Console with Instance Summary for demo-WebServer**:
   
   ![AWS Instance Summary](https://github.com/DimitryZH/terraform-webserver/assets/146372946/9b84594c-2c9b-4b25-8da2-914487a63f30)

4. **Web Browser with Apache Web Server Running**:
   
   ![Apache Web Server Running](https://github.com/DimitryZH/terraform-webserver/assets/146372946/6ef90a5b-872e-48e1-b3a9-7ed9eb2b2586)

   Ensure the webpage displays the internal IP address of the EC2 instance.

## Conclusion:
By leveraging Terraform, AWS, GitHub, and Terraform Cloud, this project showcases an efficient and automated approach to deploying infrastructure as code, facilitating consistency, repeatability, and scalability in managing cloud resources.
