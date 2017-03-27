Ansible workstaion playbook for running i3.

This will run on localhost with a local connection, make sure you have sudo rights.
Als setup become in the /etc/ansible/ansible.cfg

User the following command to run this playbook:
ansible-playbook -i inventory/workstation -bK workstation.yml -e user=$username

