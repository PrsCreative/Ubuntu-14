# Ubuntu-14 config after install

## Install Google Chrome
  $ wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
  
  $ sudo dpkg –i google-chrome-stable_current_amd64.deb

## Install Open JDK 7
  $ sudo apt-get install openjdk-7-jre 
  
  $ sudo apt-get install openjdk-7-jdk

## Duplicate database
  $ mysqldump -u root -p magento | mysql -u backup -ppassword charcoalsand;

## Dump database
  $ mysqldump -u root -ppassword mock > backup-01-10-2016-11-00.sql;
 
## Git 
  $ sudo apt-get install git
  
  $ sudo apt-get install git-gui
  
## Install Photoshop
  $ sudo apt-get install wine

## Downgrand PHP 7 to 5.5
  $ sudo apt-get purge `dpkg -l | grep php| awk '{print $2}' |tr "\n" " "`
  
  $ sudo add-apt-repository ppa:ondrej/php
  
  $ sudo apt-get update
  
  $ sudo apt-get install php5.5

## Install PHP Module Simple
  $ sudo apt-get install php5.5-mbstring php5.5-mcrypt php5.5-mysql php5.5-xml

## Remove PHP 5 All package
  $ sudo apt-get purge 'php5*' 
  
## Mysql Dump DB from SSH
  $ mysql_upgrade -u root -p --force
  
  $ service mysql restart
  
  $ mysqldump -u root -p yourdbname > /var/dbbackup/backup.sql
  
  
