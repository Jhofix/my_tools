<center><h1>MY DEV TOOLS</h1></center>

This repository contains light-weight and handy programs that I found useful when working on other projects. Every tool has been carefully developed to solve a specific problem on the go and detailed documentation has been made to make them reusable by other developers.

To use or to contribute to the tools available in this repository, kindly fork the main branch of this repository

---

<h2>List of Tools</h2>

1. deploy_loc


---
<h2>DETAILS:</h2>

1. #### deploy_loc
This is a local deployment tool which was developed in a development process to aid the deployment of website contents in the local repository directory to server path for localhost in /var/www/. Since deploy_loc uses a copy and paste approach on the local device, it is therefore suitable for copying files to any local directory.

It tries to copy the file(s) first without the super user priviledge and again with super user priviledge if the previous attempt fails. You can also set the default directory when working on a specific project so that deploy_loc automatically knows where to paste your files.

Usage:

    deploy_loc [OPTION] [PATH] FILE|DIRECTORY

OPTIONS:
    
 -s :  Use this option to set the default directory

Example: 

    deploy_loc -s my/custom/path

-d : Use this option to specify a directory to use for the current local deployment

Example: 

    deploy_loc -d directory/to/deploy/to/ file|directory

-p : Use this option to append a directory within the default directory to the path for the current local deployment

Example: 

    deploy_loc -p path/to/append/ file|directory
