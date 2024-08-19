this Assignment 2 is for the following:

Write ansible playbook to add following users in remote system, use ansible loop,
provide the list in the group_vars list, the user should be the member of devops group.
A. student1
B. student2
C. student3
D. student4


Solution:
1)  Here, I have created group in assignment.yaml file where group name with 'devops' is created with the state present.


2)  In another step, user is added with the loop where name is given with the ginger templating '{{item}}' where username is provided through the loop by creating a directory called group_vars where all.yaml file is created. Username is provided from this file to the assignment.yaml file.

Code is as below:

- name: Add group
      group:
        name: devops
        state: present

    - name: Add users
      user:
        name: "{{item}}"
        state: present
        groups: devops
      loop: "{{username}}"
