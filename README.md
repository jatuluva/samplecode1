# samplecode1
samplecode1
create a html file with name ex;script.html
esc+i edit file:

echo "hellow world from html"
echo "connecting two nodes"

save file:wq!

1. run the command:sudo cp /home/ec2-user/script.html /var/www/html/index.html 
2. command for restart: sudo systemctl restart httpd
open the public ipadress in awc ec2 : in new tab  it shows the message
3. to run the script in powershell ./<name of the file>.sh/html/etc. if access denied try with sudo ./<filename>.sh/html/etc/
4. to add user chmod +x <filename>.sh/html/etc.
5. to install telenet in powershell: after connecting to EC2: sudo yum install telnet

shell script :
#!/bin/bash
#use this for user data (Script from top bottom)
#install httpd  (linux 2 version)
 yum update
 yum install httpd
systemctl start httpd
systemctl enable httpd
echo "hellow world from SH" >>/var/www/html/index.html


to check port: guvi.in 9000


