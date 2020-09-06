Command to run current playbook in current directory :
ansible-playbook playbook.yml -i inventory.txt


Make the following changes to the /etc/apt/sources.list file to get the Ansible installation working right.

Comment the line starting deb cdrom

Uncomment bottom two lines starting deb and deb-src

Add the below two lines:

deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main
deb http://ftp.de.debian.org/debian sid main
Final file:

Once file is updated, run apt-get update and then run apt-get install ansible



OR :

sudo apt update
sudo apt install ansible