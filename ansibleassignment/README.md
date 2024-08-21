Task 1: Aug 12,: Ansible
1. Prepare two linux machines.
2. Configure ip and hostnames for each machines
A. ansible-host
B. web1.demo.com
3. Configure machines such that they can communicate with the hostname. E.g if i run ping
web1.demo.com staying in ansible-host, the machine must be reachable.
4. Configure key based ssh connection
5. Install ansible package in ansible-host machine



Solution: 


In this assignment I have maked playbook name assignment.yaml where I have installed different packages such as Chronyd, apache, also setup MYSQL server in the database using the code as in "assignment.yaml"


In the inventory file we can see that:
-web1 ansible_host=192.168.56.25 ansible_user=vagrant 
-CentOS ansible_host=192.168.56.28 ansible_user=vagrant 

these two codes are for accessing the remote server web1 and centos machine that i have acccess from my Ansible-host machcine.

