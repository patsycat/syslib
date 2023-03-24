# WordPress Installation

**Purpose:** Download and install WordPress and create a Wordpress site.

Chapter: Find instructions here: [Install Wordpress](https://cseanburns.net/WWW/systems-librarianship/17-install-wordpress.html)  

This week's assignment was a little less complicated for me, and I enjoyed learning how to set up WordPress from scratch on my own server.    

**Tasks:**  
1. Install WordPress using Customized Installation Process   
2. Create Database and User  
3. Set Up WordPress  
4. Change File Ownership  
5. Run the Install Script  
6. Finish Installation on the Website  

## Install WordPress using Customized Installation Process   

Starting on `/var/www.html` to download the latest version of WordPress using `wget`. Both download and extraction were required. This created the **wordpress** directory, so that I needed to `CD` to **/var/www/html/wordpress**.  

## Create Database and User  
This part needed to be done as the MySQL user and therefore needed to be performed in the root Linux user. At this point I stayed in the root for a long time, not needing to use `sudo` for later commands simply because I didn't switch out. But I had learned enough at this point not to be concerned about it as long as I was following instructions carefully.  

Created the new user with the appropriate commands provided and set it up with a password.  

## Set Up WordPress  

WordPress setup required creating a database, because WordPress required a database and database user to operate in Linux. Here I edited the provided `php` file to include the correct database name and password to ensure correct operation.  

## Change File Ownership  

In order to to write files to the directory, I had to run (now in my base directory) the command `sudo chown -R www-data:www-data *` and this took two tries to get it right. Typos.  

## Run the Install Script 

The last step then was to move to the browser to run the install script. Instructions were provided, and after running the script, I could use the url `http://34.171.67.164/pccblog/wp-admin/` to get to my new WordPress installation.  

The actual site is located at `http://34.171.67.164/pccblog/`.  

##  Finish Installation on the Website 

The last steps were taken on the website itself, using the admin URL to customize features and checking the preview or the actual site to see how it looked. This was a familiar task, as I had used WordPress years before.  

My only challenge this week was taken care not to have too many typos.  
 

