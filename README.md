# Steps to Provision an EC2 Instance that has Jenkins engine pre-installed on it
## Prerequisities: Knowledge of writing scripts/code using Terraform and AWS services

- #### You can use any IDE to write your terraform scripts. Visual Studio Code is the best

- #### Once your environment is set, the first thing you need to decide is, on which cloud provider are you going to provision your Infrastructure. I have decided to do this on AWS. You can always refer to Terraform documentation for any other provider reference. The details are always one Google Search away.

- #### Below are the steps to provision your infrastructure on AWS:

   - Create Your own VPC
   - Create Internet Gateway
   - Create Custom Route Table
   - Create a Subnet
   - Associate the above created subnet with Route Table
   - Create Security Group to allow ports 22, 8080, 443
   - Create a Network Interface with an IP in the subnet that was created in step 4
   - Assign an Elastic IP to the network interface created in step 7
   - Create Ubuntu server and install Jenkins 
   
- #### This repository mainly contains 2 files - Jenkins.tf and variables.tf
   
   


