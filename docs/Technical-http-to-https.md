# How to Move a Classifieds Site From HTTPS to HTTPS. 

Content:
-   What is HTTPS and why should I use it?
-   What tasks will you need to do?
    -   Get an SSL certificate and install it on your server.
    -   Go to your website’s panel to make necessary system changes.
    -   Force a redirect from HTTP to HTTPS.


In this guide, we will show you how to enable HTTPS on your classifieds site with ease.

## What is HTTPS and why should I use it?

HTTPS is the layering of HTTP on top of SSL/TLS. This basically means that the activities done on the website by users and owners are much more secure. So as a result, the HTTP traffic, including requested URLs, result pages, cookies, media and anything else sent over your HTTP connection, is encrypted when HTTPS is enabled. If an attacker is trying to interfere with your website’s connections – they cannot listen in and intercept traffic, or change it.

HTTPS is also useful for providing authentication to users of the website; it allows your visitors to identify your website and verify that it exists, is legitimate, secure and can be trusted. This level of security is compatible with search engines and their web crawlers, so adopting HTTPS indicates that you have a lot to gain.

Follow this link to read more about how and why  **[Google is also encouraging this movement](https://googleonlinesecurity.blogspot.com.es/2014/08/https-as-ranking-signal_6.html)**

## What tasks will you need to do?

1.  Get an SSL certificate and install it on your server.
2.  Go to your website’s panel to make necessary system changes.
3.  Follow this link http://yourdomain.com/oc-panel/config/update/base_url
4.  Force a redirect from HTTP to  **HTTPS.**


  

### Get an SSL certificate and install it on your server

To do this, please note that seeking for assistance from a person with the technical experience/know-how OR contacting a hosting company for installation is advised. The use of CloudFlare is also another alternative.

For a free certificate (to install it on your server), you can go to:  [www.startssl.com](http://www.startssl.com/). An example of a hosting company that offers paid certificates is Namecheap:  [www.namecheap.com/security/ssl-certificates.aspx](https://www.namecheap.com/security/ssl-certificates.aspx)

The CloudFlare alternative allows you to make use of SSL, without going through the complicated installation process. It also has a free option.

For more information on this, you can visit:  [www.cloudflare.com/ssl](https://www.cloudflare.com/ssl). Also, there is this  [tutorial for a free SSL CloudFlare certificate with Wordpress](https://wp-dreams.com/articles/2014/10/free-ssl-certificate-with-cloudflare-for-wordpress/).

Once you have the SSL certificate installed, proceed to the next step.

### Go to your website’s panel to make necessary system changes

1.  Go to your website.
2.  Login into the Admin Panel.
3.  Follow this link http://yourdomain.com/oc-panel/config/update/base_url
4.  Change the Config Value from http:// to https://
5.  Click on Submit/Save.
6.  Finally, go to Cache -> Delete All.

Once you have completed this, proceed to the next step.

### Force a redirect from HTTP to HTTPS

-   Log into your website’s cPanel.
-   Click on File Manager (and tick to show hidden files).
-   Locate your .htaccess file in the public_html directory.
-   Open the .htaccess file for editing and add the following code on the top:
    
    ```
      RewriteEngine On
      RewriteCond %{HTTPS} !=on
      RewriteRule ^$ https://%{HTTP_HOST} [L,R=301]
    
    ```
    

**Save the file and close it.**

## Short Summary

If all tasks were completed successfully, your domain name should now be prefixed with “https://” instead of “http://” whenever your website is visited.

Depending on the type of SSL certificate you installed earlier, your website should now benefit from all the other new advantages, of using SSL Encryption.

If errors are being displayed by your website, make sure that you retrace your steps; so that the troubleshooting process is easier.



*This guide is only for Yclas Self-hosted!*
