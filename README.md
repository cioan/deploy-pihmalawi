# deploy-pihmalawi
Ansible script for deploying pihmalawi

* Run the playbook on the Vagrant box:
ansible-playbook -c paramiko -i hosts deploy.yml -u emradmin --sudo

* Check playbook syntax
ansible-playbook -c paramiko -i hosts deploy.yml --syntax-check -u emradmin --sudo

* Highlights tasks that would have resulted in a change 
ansible-playbook -c paramiko -i hosts deploy.yml --check -u emradmin --sudo

* Highlights changes that would've been made to the server
ansible-playbook -c paramiko -i hosts deploy.yml --check --diff -u emradmin --sudo