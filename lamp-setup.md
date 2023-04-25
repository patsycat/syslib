# LAMP Setup  

**Purpose:** The purpose of the lAMP process is to learn how to install and configure Apache, PHP, and MySQL on a Linux server. 

Chapter: [Creating a LAMP Server](https://cseanburns.github.io/systems-librarianship/p5-creating-a-lamp-server.html)  

**Tasks:**  
1. Install Apache2  
2. Install PHP and configure that to work with Apache2  
3. Install MySQL and configured that to work with PHP and and Apache2.  

## Apache2 Installation  

 - Update system with `sudeo apt update` and `sudo apt -y upgrade`  
 - Search for Apache2 using apt using **pipe** with `sudo apt search apache2 | head`  
 - Confirm the one desired and install with `audo apt install apache2`  

### Web Page Creation, Part I  

 - Use w3m, so change directory with `cd /var/log/apache2` and install with `sudo apt install w3m`  
 - Visit the default site with `w3m 127.0.0.1` and `w3m localhost`  
 - Get the subnet/private address using `w3m 10.0.1.1` 
 - Exit w3m with `q`  

### Web Page Creation, Part II  

 - Change to `cd /var/www/html/`  
 - Back up the index by using `sudo mv index.html index.html.original`  
 - Now go to `sudo nano index.html`  
 - Set up html sample  
 - Reload the page
 - Can also view the original page by adding  `index.html.original`  

## PHP Installation  

 - Begin by using the commands `sudo apt install php libapache2-mod-php` followed by `sudo systemctl restart apache2`  
 - Check that it is running and for errors: `systemctl status apache2`  
 - Create a small php file: `cd /var/www/html/` followed by `sudo nano info.php`  
 - In the file, write sample PHP script
 - Visit the file using the extenernal IP address `/info.php` as follows: `http://34.171.67.164/info.php`  

### Configure for PHP  

 - Got to `cd /etc/apache2/mods-enabled/`  
 - Use cp command to copy with a new name: `sudo cp dir.conf dir.conf.bak`  
 - Now use `sudo nano dir.conf`  
 - Change the line I see to `DirectoryIndex index.php index.html index.cgi index.pl index.xhtml index.htm`  
 - run the `apachectl configtest` to check it and then restart `sudo systemctl reload apache2` and `sudo systemctl restart apache2`  

### Create Basic PHP Page  

 - Open an`index.php` file by using `cd /var/www/html/ and then `sudo nano index.php`
 - Add sample HTML and PHP to it
 - Save the file and exit `nano`  
 - Point to the external IP address: `http://34.171.67.164/`  

## MySQL Installation and Setup  

 - Start at `patsy@syslib-2023-pcc~$`
 - Install using `systemctl status mysql
 - Login as the **root Linux user** using `sudo su` and the command line will change to `patsy@syslib-2023-pcc:/home/patsy$`  
 - NOTE: When logged in at `root` the dollar sign becomes a pound sign `#`  
 - Type `mysql -u root` to login to mysqul  
 - Create a regular MySQL user: `create user 'opacuser'@'localhost' identified by 'xxxuse pw herexxxx';`  
 - Create database `opac.db` and then grant privileges to regular user. 
 - Remember to \q to leave MySQL user account.  
 - Practice and test commands (see chapter)  
 - Setup `login.php` file to autofill the password for the `opac.php file`  
 - Edit `opac.php`  
 - Test syntax


