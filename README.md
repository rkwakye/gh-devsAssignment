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


#To Enable HTTP on server
#update system first
sudo yum update -y
#Install Apache
sudo yum install y httpd
#install the PHP software
sudo amazon-linux-extras install -y lamp-mariadb10.2-php7.2 php7.2
#start Apache
sudo service httpd start
#make directory for website
sudo mkdir /var/www/html/
#Configure the web server to start with each system boot
sudo systemctl enable httpd
service http start
ec2-user adm wheel apache systemd-journal
sudo chown -R ec2-user:apache /var/www
sudo chmod 2775 /var/www
find /var/www -type d -exec sudo chmod 2775 {} \;
find /var/www -type f -exec sudo chmod 0664 {} \;
cd /var/www
sudo mkdir inc
sudo cd inc
echo "<h1><h>Welcome to GH-Devs"</b></h1>">/var/www/html/index.html
 
