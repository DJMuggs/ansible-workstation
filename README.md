Ansible playbook for running Fedora 25 with i3 on a Lenovo T540p.
This includes the bumblebee driver for nvidia and fix the wireless perfomance of the Intel(R) Centrino(R) Advanced-N 6235 AGN.
Will replace i3status with i3blocks and setup i3blocks for you.

In the playbook are some settings and features that i find usefull for my own workflow.
Feel free to fork this repository and set things up the way you like.

This will run on localhost with a local connection, make sure you have sudo rights.

Also setup become in the /etc/ansible/ansible.cfg


Use the following command to run this playbook:

ansible-playbook -i inventory/workstation -bK workstation.yml -e user=$username

