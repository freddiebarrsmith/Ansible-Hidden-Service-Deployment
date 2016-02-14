Setup Instructions
===================================
apt-get update

echo "localhost ansible_connection=local" >> /etc/ansible/hosts 

apt-get -y install ansible

apt-get -y install git

git clone https://github.com/freddiebarrsmith/Ansible-Hidden-Service-Deployment.git

ansible-playbook darkweb.yml


cat /home/tordir/hostname 

this last command is to get the name of your new .onion site!
