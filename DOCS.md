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

