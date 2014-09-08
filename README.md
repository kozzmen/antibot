#antiBot


Single Script that protects any other php script avoiding brute force attacks to it.

#####Screen capture
![alt text](https://raw.githubusercontent.com/masterguru/antibot/master/antibot.png "Antibot capture")


##How to use (i.e. in a WordPress site)

 1. Download [antibot.php](https://raw.githubusercontent.com/masterguru/antibot/master/antibot.php "antibot.php raw script") and put it in same folder than the script you want to protect (i.e. wp-login.php)
 2. Edit your php script and add this line on top of it:

  ```php
  <?php include('antibot.php'); ?>
  ```
 3. Save changes.

##What happens next?

* Next time that wp-login.php will be called then this script will be loaded first and it will ask to click a button to continue.

* At same time it will be returning an HTTP header with 404 error code to frustrate possible robots/bots/scrappers about if it exists or not. 

##Is it useful?

* Most of times these bots decide to abandon the site, despite others insist in execute a brute force login attack, but thanks to this protection, it use minimal server resources because it blocks a full Wordpress load. 

* If you are not using this script and you are suffering a brute force attack, then Wordpress has to execute too many steps to deny the access, forcing your server to spend more resources, and causing DDOS problems if there are several bots at same time.

I hope you like it! It has helped some of my servers full of Wordpress/Joomla sites to run better.

