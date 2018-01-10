# Linux-Patch-Management

root@master_ubuntu1604server:~/playbooks# cat /etc/ansible/hosts


[linux-dev-servers]


testserver1


testserver2



root@master_ubuntu1604server:~/playbooks# ansible-playbook -i /etc/ansible/hosts --syntax-check linux_patch_install.yml




root@master_ubuntu1604server:~/playbooks# ansible-playbook -i /etc/ansible/hosts -l linux-dev-servers linux_patch_install.yml
