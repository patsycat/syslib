# Cataloging Module  

**Purpose:** Complete another module for a barebones ILS (Integrated Library System).  

Chapter: Find instructions here: [Creating a Bare Bones OPAC](https://cseanburns.net/WWW/systems-librarianship/16.8-basic-opac-admin.html)    

**Tasks:**  
1. Create an `index.html` file in a new cataloging directory in `var/www/html`  
2. Create an `insert.php file` in the new cataloging director  
3. Secure the cataloging directory with the `htpasswd` command  
4. Add additional records using the new web form  
5. Use the OPAC to retrieve the new records  

## Create an `index.html` file in a new cataloging directory in `var/www/html`  

This was a simple process and one that I finally didn't need to look up! I did a cd to `var/www/html` and then created the directory with the 'sudo mkdir cataloginng' command, then (once I changed to that directory) I created the file with the command `sudo nano index.html`. Content was copy-pasta from the instructions.   

## Create an `insert.php file` in the new cataloging directory  

This was also simple, as I've learned the commands necessary and it does not include creating my own php. This file was created as sudo nano index.html in the same directory. Here, we have the commands that will complete the serach and return it to the HTML-based page.  

## Secure the cataloging directory with the `htpasswd` command  

This was a little more tricky, but instructions were very straightforward. In this section, I created a user name and password for entering books into the OPAC. The authentication was created via a file in `/etc/apache2`. At one point I used the wrong copy-pasta and ended up with some messages that made no sense, but it only took a return to the instructions to see that I'd accidentally skipped ahead. Once I had the right information in place, everything worked perfectly.

## Add additional records using the new web form  

I've been raiding my Goodreads list to pull books I've read into the records. Data entry worked like a charm, once I typed my password correctly.  

## Use the OPAC to retrieve the new records  

Again, simple to do through the HTML interface.  

**Additional Thoughts**  
This week was the first time I really felt pretty efficient at what we were doing. I could enter commands and understand what I was doing with more confidence. Even with more than a week's absence due to a storm outage at my home and the post-outage work we had to do, I sat down and easily got back into it. That was a relief.  
