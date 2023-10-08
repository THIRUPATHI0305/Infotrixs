# Infotrixs
Step 1: Launch an EC2 Instance
Log in to your AWS Management Console.
Go to the EC2 Dashboard and click "Launch Instance."
Select an Ubuntu AMI 
Choose a t2.micro instance type.
Configure the instance details.
Configure security groups for your instance. Open ports 22 (SSH), 80 (HTTP), and 3306 (MySQL) for the MySQL server. You can restrict these 

Step 2: Install and Configure MySQL
SSH into your EC2 instance using your private key.
Update the package list: sudo apt update
Install MySQL Server: sudo apt install MySQL-server
During the installation, set the MySQL root password.
Secure your MySQL installation: sudo mysql_secure_installation
Create a MySQL database and user for WordPress.

Step 3: Install and Configure WordPress
Install Apache web server and PHP: sudo apt install apache2 php libapache2-mod-php php-MySQL

Download WordPress and configure it:
Download WordPress: wget https://wordpress.org/latest.zip
Extract it: unzip latest.zip
Move the WordPress files to the web server directory: sudo mv wordpress/* /var/www/html/
Configure the WordPress database settings in wp-config.php.
Change the ownership of the WordPress files to the webserver user: sudo chown -R www-data:www-data /var/www/html
Restart Apache: sudo systemctl restart apache2

Step 4: Create a Welcome Page
Access your WordPress site in a web browser.
Aws Instance : 

 
Security Group:
 
Output:

 

Url : welcome 
ip : 3.81.79.34

