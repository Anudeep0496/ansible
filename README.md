# ansible<br>
<h1>ansible</h1>h1><br>
Create a File:<br>
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b <br>

Copy file:<br>
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b<br>
