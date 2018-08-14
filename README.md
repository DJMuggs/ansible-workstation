# Ansible playbook Fedora Workstation 26+
This ansible playbook is for running Fedora 26+ or higher with i3 on a Lenovo T540p.  
This includes the bumblebee driver for nvidia and fix the wireless perfomance of the Intel(R) Centrino(R) Advanced-N 6235 AGN.  
The playbook will replace i3status with polybar and setup polybar for you.

In the playbook are some settings and features that i find usefull for my own workflow.  
Feel free to fork this repository and set things up the way you like.

This will run on localhost with a local connection, make sure you have sudo rights.

##### Prequisites
The following software is required for this ansible playbook to work.

- git
- ansible

##### Run the playbook
Use the following command to run this playbook:

`ansible-playbook -i inventory/workstation -K workstation.yml -e user=$username`

##### Extras
There is also an backup and restore playbook for your prescious data.  
Set the location and fstype of your backup disk and start

`ansible-playbook -i inventory/workstation -K backup.yml -e user=$username -e disk=$disk -e fstype=$fstype`
