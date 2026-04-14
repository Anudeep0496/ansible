# ansible<br>
<br>
<br>
<h2>Create a File:</h2><br>
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b <br>

<h2>Copy file:</h2><br>
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b<br>
