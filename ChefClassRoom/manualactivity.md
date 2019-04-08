## Lamp Stack

* This is for deploying any php applications
* Google result [here](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04)

### Steps
```
sudo apt-get update
sudo apt-get install apache2 -y
# http://<publicip>
sudo apt-get install php libapache2-mod-php php-mcrypt php-mysql
sudo systemctl restart apache2
sudo apt-get install php-cli
sudo nano /var/www/html/info.php
# <?php
# phpinfo();
# ?>
```

### Execute
* Execute all the above commands manually