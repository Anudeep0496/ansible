# ansible
ansible
Create a File:
ansible web -i inventory.ini -m file -a "path=~/anudeep.txt state=touch" -b

Copy file
ansible web -i inventory.ini -m copy -a "src=index.html dest=~/" -b
