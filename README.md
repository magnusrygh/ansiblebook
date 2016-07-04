Testing Ansible
---------------
check the SSH port and private_key path by using: |
 vagrant ssh-config 

Update ansible.cfg with ssh_host, ssh_port, and identity file if needed

run: ansible webservers -m ping

run: ansible-playbook playbook.yml

run: ansible testserver -m setup -a 'filter=ansible_python'
