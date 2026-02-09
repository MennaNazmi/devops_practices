systemctl status mariadb.service >> checking the eroor 

the issue is in the logs file as missind data directory and uninit database

❌ Directory doesn't exist
❌ Wrong ownership (not mysql:mysql)
❌ Empty directory (uninitialized database)


create a directory 
sudo mkdir /var/lib/mysql


giving premissions 
sudo chown -R mysql:mysql /var/lib/mysql
sudo chmod -R 0700 /var/lib/mysql


sudo mariadb-install-db --user=mysql --datadir=/var/lib/mysql


