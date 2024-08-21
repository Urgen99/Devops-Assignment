 Add the ssh banner in the remote hosts with the following contents, the sshd service
should restart only if there is change in the sshd_config. Hintz use ansible handlers
This {{ansible_distribution}} is managed by Ansible





In this assigment as we can see in the assignment.yaml file, banner file is added to the destinatin: /etc/motd directory with the message :  "This {{ansible_distribution}} is managed by Ansible \n"

after that sshd config file is updated. Also handlers is used to restart the ntp service on CentOS.
