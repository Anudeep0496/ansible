# ansible<br>
<br>
<br>
<h3>Create a File:</h3>
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b <br>

<h3>Copy file:</h3>
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b<br>

<h3>To check the syntax of playbook:</h3>
ansible-playbook --syntax-check 05-playbook.yaml<br>
