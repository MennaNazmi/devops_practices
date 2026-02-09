# login to server 3
ssh banner@172.16.238.12

# detect the os release
cat /etc/os-release

# step 1: install zip 
sudo yum install zip
# step 2: create zip  
zip -r xfusioncorp_news.zip /var/www/html/news
# step3 : copy to remote backup server
scp xfusioncorp_news.zip clint@stbkp01:/backup/

# step4 : create the bash file
vi f.sh >> im inside the file now

        #!/bin/bash
        zip -r xfusioncorp_news.zip /var/www/html/news
        scp xfusioncorp_news.zip clint@stbkp01:/backup/


# step5: make the file executable
chmod +x /scripts/ecommerce_backup.sh

# step 6:  Do not use sudo inside the script
generate a key  >>ssh-keygen -t rsa

copy the key to the remote server >> ssh-copy-id tony@172.16.238.10

>> ssh-copy-id steve@172.16.238.11

>> ssh-copy-id banner@172.16.238.12
>> ssh-copy-id clint@stbkp01  --> backup server
# step 7: open crontab

0 0 * * 0 /scripts/news_backup.sh

# step 8: verify its saved 
crontab -l

