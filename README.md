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

## Downgrand PHP 7 to 5.6
  $ sudo apt-get purge `dpkg -l | grep php| awk '{print $2}' |tr "\n" " "`
  
  $ sudo add-apt-repository ppa:ondrej/php
  
  $ sudo apt-get update
  
  $ sudo apt-get install php5.6

## Install PHP Module Simple
  $ sudo apt-get install php5.6-mbstring php5.6-mcrypt php5.6-mysql php5.6-xml
