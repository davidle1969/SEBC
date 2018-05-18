sudo yum install mariadb-server -y
sudo service mariadb stop
stop mariadb.service
sudo vi /etc/my.cnf
sudo systemctl enable mariadb
sudo service mariadb start
