Setup Instructions
===================================
apt-get update


apt-get -y install ansible

echo "localhost ansible_connection=local" >> /etc/ansible/hosts 


apt-get -y install git

git clone https://github.com/freddiebarrsmith/Ansible-Hidden-Service-Deployment.git

ansible-playbook Ansible-Hidden-Service-Deployment/darkweb.yml


cat /home/tordir/hostname 

this last command is to get the name of your new .onion site!

Stuff I'm Working On
===================================

Bash Deployment
OS Hardening

Bash Deployment One Liner (Courtesy of ryanlol on ycombinator)
===================================
  curl 'https://raw.githubusercontent.com/freddiebarrsmith/Ansible-Hidden-Service-Deployment/master/darkweb.yml' |grep -elinein -ecommand -e action|sed -e 's/command//' -e 's/action://' -e 's/  //g' -e 's/: //' -e 's/lineinfil.*t=/cat >>/' -e 's/line=/<<</' -e 's/ pkg=/-get -y --force-yes install /' -e 's/state=latest//' -e 's/t u/t-get -y u/' -e 's/_cache=yes//'
