# ansible<br>
<br>
<br>
<h3>Create a File:</h3>
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b <br>

<h3>Copy file:</h3>
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b<br>
