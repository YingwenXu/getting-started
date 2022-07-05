Role Name
=========
docker_install
role for install common tools on remote servers, and deploy docker and docker-compose, then copy getting-started.tar to remote nodes and run it export port 3000:3000

Requirements
------------
ansible config under: /home/ywxu/ansible/ folder, and inventory must be spcified 
hosts can be specified as your request under /home/ywxu/ansible/inventory
set ssh-key for user: ywxu from ansible control to other nodes specified in your inventory, and exec ansible-playbook use ywxu user

Role Variables
--------------
docker compose version defined and can changed under: /home/ywxu/ansible/roles/docker_install/vars/main.yml  

------------
all useful yaml:
under:
/home/ywxu/ansible/roles/docker_install/tasks/
have four sub tasks:
main.yml
prepare.yml
install.yml
todo_app.yml

Author: Yingwen Xu
-------------------
