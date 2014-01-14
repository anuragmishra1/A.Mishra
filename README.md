
Start-Up-Services
=================

For Kazoo
=========


In this, kazoo start when system start with the user kazoo with daemon. So, when anyone will use this script add user name kazoo in their system(Ubuntu). 

The process of adding user run these commands: 
  "adduser --system kazoo"
  "addgroup --system kazoo"

After that edit in "vi /etc/passwd" at the last where you will see kazoo change the groupId write appropriate groupId which is given by system when you create the group and change /home/kazoo to /opt/kazoo and save.

Then copy this script file as name "kazoo" and paste in folder /etc/init.d/.

Then run "sudo apt-get install sysv-rc-conf" after that run "sysv-rc-conf kazoo on".Then it will be run with the daemon process.
