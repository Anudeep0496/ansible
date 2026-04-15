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
