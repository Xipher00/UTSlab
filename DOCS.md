# Lab Test
## Package Installation
1. sudo apt install nginx
2. sudo apt install mariadb-server
3. sudo apt install mariadb-client
4. sudo apt install php7.2
5. sudo apt install php7.2-fpm 
6. sudo apt update 
7. sudo service nginx start
8. sudo service mysql start
9. sudo service php7.2-fpm start
10. sudo mysql_secure_installation
11. sudo apt install curl
12. sudo apt curl -4 icanhazip.com
13. sudo service nginx status
14. sudo service mysql status
15. sudo service php7.2-fpm status

## Nginx Server Setup
1. ls 
2. cd ..
3. ls
4. cd ..
5. ls
6. cd /etc/nginx/sites-available/
7. ls
8. sudo cp default midtest
9. sudo nano midtest
10. remove default_server, remove [::]80 default_server, add index.php before index.html, uncomment \.php block, change version of php to 7.2, uncomment /\.ht block
11. sudo nginx -t
12. sudo ln is /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled
13. sudo unlink /etc/nginx/sites-enabled/default
14. sudo service nginx reload
15. cd..
16. cd..
17. cd.. 
18. cd /var/www/html
19. sudo nano info.php
20. paste <?php phpinfo(); ?>
21. open localhost/info.php in your browser
22. sudo rm info.php

## Lion Wiki
1. sudo wget http://lionwiki.0o.cz/download/3.2.11/lionwiki-3.2.11.zip
2. sudo unzip lionwiki-3.2.11.zip
3. cd lionwiki-3.2.11/
4. sudo cp -r lionwiki-3.2.11.zip /var/www/html
5. sudo rm -rf index.html
6. sudo rm -rf index.nginx-debian.html
7. sudo cp -r config.php /var/www/html
8. sudo cp -r index.php /var/www/html
9. sudo cp -r lang /var/www/html
10. sudo cp -r plugins /var/www/html
11. sudo cp -r templates /var/www/html
12. sudo cp -r var /var/www/html
13. sudo chmod 777 ./var
14. Now we edit the main page, add the information about ourselves on the wiki