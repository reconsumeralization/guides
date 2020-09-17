# Docker configuration for Yclas Self Hosted


The following guide describes how you can use a docker image to install Yclas Self Hosted.

### What is installed

-   Official Ubuntu Server 14.04 LTS (Trusty Tahr) builds
-   Apache2
    -   PHP 7
    -   cURL
    -   GD
    -   mysqli
    -   mcrypt
    -   apcu
-   MySQL 5.5
-   phpmyadmin
-   Installation file for the latest Yclas Self Hosted

### Instructions

1.  Install  [Docker].(https://docs.docker.com/installation/)
2.  Clone this repo:
    
    ```
     git clone https://github.com/yclas/docker.git
    
    ```
    
3.  Stop apache2 and mysql:
    
    ```
     sudo service apache2 stop
     sudo service mysql stop
    
    ```
    
4.  Run the container:
    
    ```
     sudo docker run -t -i -p 80:80 -p 3306:3306 kotsios/env:latest /bin/bash
    
    ```
    
5.  Start apache2, mysql and postfix:
    
    ```
     sudo service apache2 start
     sudo service mysql start
     sudo service postfix start
    
    ```
    
6.  Load on your browser:
    
    ```
     http://reoc.lo/install-yclas.php
    
    ```
    
7.  Install Yclas Self Hosted using these:
    
    ```
     Database name: openclassifieds
     User name: root 
     Password: 1234
    ```
