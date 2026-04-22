# ansible<br>
<br>
<br>
<h3>Create a File:</h3>
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b <br>

<h3>Copy file:</h3>
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b<br>

<h3>To check the syntax of playbook:</h3>
ansible-playbook --syntax-check 05-playbook.yaml<br>

<h3>Command to pass the Vars by Arguments</h3>
ansible-playbook -i inventory.ini 11-Args-Vars.yaml -e "auth=Anudeep" -e "course=Ansible" -e "learn=Devops"<br>

<h3>Preference of Printing the Variables</h3><br>
1. Arguments
2. Tasks
3. Files
4. Prompt
5. Play
6. Inventory

<h3>ansible vault </h3> <br>
ansible-vault create <file-name>.yaml<br>

create servers<br>
de commissiong ansible vault and replace with secret manager or paramter store<br>

=====<br>
Ansible static inventory<br>
==========================<br>
inventory --> a list of hosts and groups, this is static <br>

Dynamic --> when traffic increases, servers should be increased, when traffic decrased servers should be terminated<br>

dynamic inventory<br>
=================<br>
ansible can connect to dynamic environments like cloud aws, azure, gcp, etc. It has to query the servers based on the parameters we give<br>

ssh-keygen -t rsa<br>


<h3>Ad-hoc Commands</h3>
ansible all -i inventory.ini -b -m service -a "name=nginx state=started"<br>

ansible all -i inventory.ini -m shell -a "systemctl status nginx"<br>


