# OPAC Setup

**Purpose:** Learn the way data from a relational database is retrieved and entered using various technologies.

Chapter: Find instructions here: [Creating a Bare Bones OPAC](https://cseanburns.net/WWW/systems-librarianship/16.5-basic-opac.html)  

This week I understand that we are supposed to be more journaling understanding rather than only documenting process, which means something different to me. Changing up my format somewhat.  

**Tasks:**  
1. Create the HTML Page  
2. Create a PHP Search Script  

## Create the HTML Page  

Starting on `/var/www/html` to create an HTML page with the command `sudo nano opacbb.html`. Here I'm creating a page that will essentially serve as an interface to the database. 

Within the html will be a call-out of sorts to the PHP script, which will run to fetch the items sought. As learned last week, any information can be pulled and ordered based on need; this week it is more about creating 
and simple form via HTML to pull information into a listing output such as may be presented in easily read format to a patron. The HTML is the method for presenting the form and the output into the easily read format.   

After copying and pasting the HTML code, I returned to mysql to use opacdb and create more records. I pulled up my Goodreads page and grabbed a few books off my list to enter into the database.  

I found myself having to review previous instructions and my documentation to ensure I was in the right place using the right commands. It's a lot to remember for a newbie. On the other hand, it's good practice.  

## Create a PHP Search Script  

The script provides the commands that run out and fetch what we need in the database, returning it to the easily read HTML page. Using the command 'sudo nano search.php` I am able to copy and paste the php code.  

This was fairly easy, but the challenge I found was that the html file returned me to opacbb.php and not opacbb.html. It wasn't difficult to determine that this was the error and that I could both correct it by hand in the browser window and by correcting the html file iteself.  
