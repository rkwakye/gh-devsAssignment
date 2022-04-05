# gh-devsAssignment
Gh-DevsAssignment Create VPC with 2 AZ's, add database on EC2 and use load balancer

This is for homework assignment
Company Name (gh-devs), regions (us-east-2), software (wordpress)


1. Create VPC, Private & Public Subnets, Routes etc… for a company to deploy
    -Screenshot of VPC created, showing both private and public subnets, show the routes.
    - Create Security Groups for All-Internet AND security group for SSH on port 22
    - Take Screenshot
    - Created ec2 instance named wordpress
    - ssh'ed into it and installed wordpress using command line
    - configured wordpress on wordpressEC2
    - installed apache2 on wordpressEC2
    - alternatively Amazon a free tiered serive to create an mySQL EC2 
2. Database (Mysql RDS)
    - screenshot of terminal lines executed to create MySQL RDS
3. Autoscaling group of wordpress instances preconfigure with your ansible playbook
     Launch template
     Auto Scaling group
     Configure AG instances to connect to RDS instance
4. Load balancer
      Launch LB
      Configure LB
