Testing Ansible
---------------
check the SSH port and private_key path by using: 
 vagrant ssh-config 

Update ansible.cfg with ssh_host, ssh_port, and identity file if neededjango
run: ansible testallservers -m ping
run: ansible django -a "date"

run: ansible all -a "date"

ansible-playbook builtinvars.yml -e greeting=hey -e @varfile
