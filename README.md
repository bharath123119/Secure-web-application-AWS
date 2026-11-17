# Secure Web Application on AWS

## Project Overview
Built and configured a secure web application on AWS using two EC2 web servers deployed in private subnets and an Application Load Balancer as the public entry point.

## Architecture
- Application Load Balancer in public subnets.
- Two EC2 web servers in private subnets.
- Nginx installed on both EC2 instances.
- Server 1 hosts a Home Page.
- Server 2 hosts a Personal Page.
- Separate security groups for the Load Balancer and web servers.
- Target groups configured with HTTP health checks.

## Technologies Used
- AWS EC2
- Application Load Balancer (ALB)
- VPC and Subnets
- Security Groups
- Nginx
- HTML

## Security Configuration
- ALB accepts HTTP traffic from the internet.
- EC2 instances accept HTTP traffic only from the ALB security group.
- Web servers are deployed in private subnets.

## Application Pages
- Home Page – Server 1
- Personal Page – Server 2

## Testing
- Verified Nginx service on both servers.
- Tested HTML pages using curl.
- Configured ALB target group health checks.
- Verified load balancing through the ALB DNS name.

## Learning Outcomes
- AWS networking and subnet configuration.
- Security group management.
- Application Load Balancer configuration.
- Private EC2 deployment.
- Nginx web server configuration.