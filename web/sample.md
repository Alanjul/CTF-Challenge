#Sample web challege

Problem
![alt text](image-1.png)

Tools: web browser for manual testing

step 1. Launch the website
![alt text](image-2.png)
Approach
. I first create php file and upload on the profile picture
I made the php file and upload to web ![alt text](image-3.png)
![alt text](image-4.png)
After uploading, The file file1.php has been uploaded Path: uploads/file1.php  was displayed
I modified the web link from http://standard-pizzas.picoctf.net:56436/upload.php
to http://standard-pizzas.picoctf.net:56436/uploads/file1.php that shows the website have unrestricted file upload that exposes it  remote code execution
![alt text](image-5.png)

create another PHP file  to allow me enter commands to traverse the files in the website
![alt text](image-6.png)
when I try sudo shows you don't need a password to run any commands on the website
![alt text](image-7.png)
Then add sudo as shown below  ls /root and flag.txt was found
![alt text](image-8.png)
Then I run the sudo cat /root/flag.txt in website