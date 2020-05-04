### Introduction
This is a terraform project to deploy `Nginx` container on ECS fargate cluster. This will create the following resources in AWS:
 * VPC, subnets
 * Security groups
 * ECS Fargate cluster
 * ALB, Target-group
 * Log group

### How To Run
* Clone this repository
* Make sure you have terraform installed
* Make sure, AWS credentials are set in `~/.aws/credentials`
* Run `terraform init` to initialize this as terraform repository
* Run `terraform plan` to see what all resources are going to get created
* Run `terraform apply` to actually create the resources

### Output
Once you have created the infrastructure, its going to output the ALB endpoint to access the deployed Nginx container.