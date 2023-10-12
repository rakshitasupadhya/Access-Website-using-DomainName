# Access-Website-using-DomainName
This is a simple demonstartaion on how to acces the website hosted on EC2 using Domain name created by Route53 &amp; Elastic Load balancer

# AWS services:
1. Amazon Elastic Compute Cloud (Amazon EC2)
2. Elastic Load Balancer
3. Route53

# Implementation
1. Launch EC2 instance  (Install httpd)
   •	Select VPC and subnet
   •	Select Security group as http
   •	Install httpd as bootstrap when server is started
2.	Create Application Load Balancer
   •	Select the security group & VPC created during EC2 
   •	Configure EC2 instance as target
3. Open the DNS name link under ALB and see the following results.
   Note: This URL is not user friendly hence Route53 is used to create a user friendly URL to access website
4.	Configure Route 53 Alias
   •	Map a friendly domain name to application load balancer so we can access our website using our own domain name 
    Note: Hosted zone acts as a container to all domain names
5. Go to hosted names and create record
6. Copy the record name and open in new tab



