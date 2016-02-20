# Setup Instructions

```sh
apt-get update
apt-get -y install ansible
echo "localhost ansible_connection=local" >> /etc/ansible/hosts 
apt-get -y install git
git clone https://github.com/freddiebarrsmith/Ansible-Hidden-Service-Deployment.git
ansible-playbook Ansible-Hidden-Service-Deployment/darkweb.yml
cat /home/tordir/hostname 
```
The last command is to get the name of your new .onion site!

# Stuff I'm Working On

* Bash Deployment
* OS Hardening
