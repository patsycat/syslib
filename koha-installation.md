# Koha Installation

**Purpose:** Download and install Koha and create the basis for an Integrated Library Service (ILS).

Chapter: Find instructions here: [Install Koha ILS](https://cseanburns.github.io/systems-librarianship/20-install-koha.html)  

This week's documentation is dedicated to all the things I forgot! This task was very much like Wordpress but enough time had elapsed that I needed to review things and enough was different that I had to think through those differences one by one.   

**Tasks:**  
1. Server Setup  
2. Install Koha  
3. Configure Koha 
4. Koha Web Installer
5. Run the Install Script
6. Finish Installation on the Website  

## Server Setup

We had to install a more robust server, so we returned to Google Cloud and set up another instance. This was fairly easy, as we done it once before. I now have two notes on my desktop for logging into servers, because each one requires a different copy-paste into my google cloud connection. One at a time, of course; only using one at once. Extra steps included adding a Koha repository and then downloading Koha with `wget` to the new server.

## Install Koha  

Installation was easy but took about 5 minutes using `apt install koha-common`.

## Configure Koha
Configuration was not difficult but took a number of steps. I almost skipped a step twice and caught myself. Instructions were very straightforward.

## Koha Web Installer  

This required pulling the username and password from `/etc/koha/sites/bibliolib/koha-conf.xml` in the `<config>` line before heading to the web interface.

## Run the Install Script 

Took me to the website to complete setup at `http://34.70.98.40:8080/`  

The actual site is located at `http://34.70.98.40`.  

##  Finish Installation on the Website 

The last part of setup was on the website. After setting up the site, I added a few patrons, a couple of books, and then checked out a book to a patron. Checking out was a little difficult, but I finally realized I needed to set a barcode for each book, and once I learned how to do that from the manual, I was all set for checkout. I then took some screenshots and spent some time learning how to delete a circulation history. I actually ended up anonymizing circulation history. As a last bit, I added some CSS to create a different color background for the patron-facing search.
