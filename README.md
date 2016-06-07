Testing Ansible
---------------
check the SSH port and private_key path by using: |
 vagrant ssh-config 

Update ansible.cfg if needed

run: ansible webservers -m ping

run: ansible-playbook playbook.yml

