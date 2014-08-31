
Start-Up-Services
=================

For Kazoo
=========


With the  using this script kazoo will automatically start when your system starts, but this script only for Ubuntu OS. To use this script you need to create a user 'kazoo'.
 
The commands are below to add user in Ubuntu:
  adduser --system kazoo
  addgroup --system kazoo

After adding the user 'kazoo', please edit file /etc/passwd in the last of this file you will see kazoo user like as below:
  kazoo:x:1001:1001:kazoo:/home/kazoo:/bin/bash

Change /home/kazoo to /opt/kazoo in above line. After that copy the kazoo script and paste it in the /etc/init.d/ folder and make sure copied script has a execute permission.

To give the execute permission you need to run below command in /etc/init.d/ folder
  chmod +x kazoo

Install 'sysv-rc-conf' by using below command:
sudo apt-get install sysv-rc-conf

If you have already installed 'sysv-rc-conf' in your system then run the below command:
sysv-rc-conf kazoo on

Restart your system and you will see kazoo will start automatically when the system starts.
