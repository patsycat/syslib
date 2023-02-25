# Git and GitHub Setup

## GitHub Setup
1. [On GitHub.com](https://github.com/)
2. Set up GitHub account with personal email. (Make private in settings.)
3. Create an SSH key on Linux server with the command found below. Use the email used to sign up for GitHub, surrounded with double-quotes.

    `ssh-keygen -t ed25519 -C "myemail@email.com"`

4. Add SSH public key to GitHub. To add public key to GitHub:
    - Go to Settings **SSH and GPG keys**
    - Click on **New SSH key**
    - On Linux server, use nano to open the file: **~/.ssh/id_ed25519.pub**
    - Copy contents
    - Paste contents into the **New SSH key** text box on GitHub.
5. Create a new repository. Name: **syslib**

More documentation on GitHub:  
https://docs.github.com/en  
[How to create ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Set Up Git

On the Linux server:

Configure git on the remote server

1. Configure identity and other defaults. From the command prompt:  
`git config --global user.name "First Name Last Name"`  
`git config --global user.email "firstlast@example.com"`  
`git config --global core.editor nano`  
`git config --global init.defaultBranch main`

2. Check the settings:  
`git config --list`

More `git` documentation available:  
https://git-scm.com/

## Use Git on Remote Server

On the Linux server:  

Make new directory in the home directory. Name: **repos**  
Change into the new directory with cd command  
Get the git URL from the green **Code** dropdown box on the GitHub repo site.  
Clone using the repo using the following command:  

`git clone git@github.com:patsycat/repos.git`  

Add files in cloned repo.  

Track changes with: `git add .`  
Commit changes and add message with: `git commit -m "add message in quotes"`  
Push changes to remote repo with: `git push origin main`  

Going forward, update by using these commands to sync the local repo to the GitHub repo:  

`git add .`  
`git commit -m "add message in quotes"`  
`git push origin main`

## Editing on GitHub

When editing a file on GitHub, to syn to the local repo on the Linux server, use the following command:  

`git pull origin main`

# Markdown

Visit Markdown documentation here:  

[Markdown Documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)  
[Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
