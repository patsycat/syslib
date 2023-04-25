# OMEKA Installation

**Purpose:** Download and install OMEKA and create an OMEKA collection site.

Chapter: Find instructions here: [Install Omeka](https://cseanburns.github.io/systems-librarianship/18-install-omeka.html)  

This week's documentation is dedicated to all the things I forgot! This task was very much like Wordpress but enough time had elapsed that I needed to review things and enough was different that I had to think through those differences one by one.   

**Tasks:**  
1. Complete prep steps  
2. Unzip and install Omeka   
3. Create Database and User  
4. Change File Ownership    
6. Finish Installation on the Website  

## Complete prep steps

Here I forgot to install items the instructor provided in an announcement. I just ... forgot. As a result, my Omeka webpage presented an error after my last step. After installing, I refreshed and got the Omeka setup screen in the webpage. Otherwise, I followed the steps to install imagemagick, enable `mod-rewrite` and restart Apache. 

## Unzip and install Omeka  

Because I forgot to install the announced items I did not have an unzip to run. I went out to GeeksforGeeks (what a great site) and found the commands to download and use unzip. I then unzipped Omeka and renamed it's directory to `Omeka`. During this step I consistently forgot to use `sudo`.

## Create Database and User  
This part was easier, but because it involved Mysql and the root directory, I reread all instructions carefully.  

Created the new user with the appropriate commands provided and set it up with a password, then restarted.  

Also moved into the directory to open db.ini and insert the host (localhost), user db, user name, password. It took a while to remember what went where, and previous chat in Element helped keep me on the right track. Eventually I did find a typo in my list and almost went cross-eyed before I found it.  

## Change File Ownership  

Used the CHOWN command to change ownership, like last week.  

## Run the Install Script 

Took me to the website to complete setup at http://34.171.67.164/omeka/admin  

The actual site is located at http://34.171.67.164/omeka/.  

##  Finish Installation on the Website 

The last steps were taken on the website itself. I set the theme and created a Collection and added Items. I used LOC to select subject terms and the Dublin Core definitions to enter my information. This part was fun.  
