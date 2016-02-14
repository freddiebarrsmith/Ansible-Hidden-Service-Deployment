Setup Instructions
===================================
apt-get update

echo "localhost ansible_connection=local" >> /etc/ansible/hosts 

apt-get install ansible

apt-get install git

git clone https://github.com/freddiebarrsmith/Ansible-Hidden-Service-Deployment.git

ansible-playbook darkweb.yml





