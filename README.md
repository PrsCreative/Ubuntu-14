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

