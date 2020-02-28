#LAB TEST MICHELLE EVALISTA PATRICIA - JEFREY VINSON CHEN#

#MICHELLE as administrator
#JEFREY as documenter

#Step 1 : Package Installation
sudo apt install nginx 
sudo apt update 
sudo apt install mariadb-server 
sudo apt update 
sudo apt install mariadb-client 
sudo apt update 
sudo apt install php7.2
sudo apt update
sudo apt install php7.2-fpm
sudo apt update

Restart

sudo service nginx enable
sudo service nginx start
sudo service mysql enable
sudo service mysql start
sudo service php7.2-fpm enable
sudo service php7.2-fpm start

curl -4 icanhazip.com 
sudo mysql_secure_installation
 
#Step2: Nginx Server Setup
cd etc/nginx/sites-available
sudo cp default midtest
sudo nano midtest
#1.Listen 80;
#2.Add index.php, right before index.html
#3.Uncomment ~\.php$
#4.Change the FPM version from 7.0 to 7.2
#5. Uncomment location ~/\.ht
sudo nginx -t
sudo ls -s /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/
sudo unlink /etc/nginx/sites-enabled/default
sudo service nginx reload
cd var/www/html
sudo nano info.php
sudo rm info.php
