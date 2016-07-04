Testing Ansible
---------------
check the SSH port and private_key path by using: |
 vagrant ssh-config 

Update ansible.cfg with ssh_host, ssh_port, and identity file if needed

run: ansible vagrant -m ping

run: ansible-playbook playbook.yml

for "fun": ansible all -a "date"
