malis3--00

ssh -l malis3-qa 192.168.1.150

scp hysteryale.war malis3-qa@192.168.1.150://home/malis3-qa/Desktop/hysteryale/be-deployment/apache-tomcat-9.0.80/webapps


scp hysteryale.war malis3-qa@192.168.1.150://opt/tomcat/latest/webapps



scp .env malis3-qa@192.168.1.150://home/malis3-qa/Documents/

scp import_files.zip malis3-qa@192.168.1.150://home/malis3-qa/Documents

netstat -ano | grep ":3005"

* kiem tra ung dung nao dang su dung port

sudo netstat -lpn |grep :8080
tcp6       0      0 :::8080                 :::*                    LISTEN      31367/java   

+ dong port 
sudo kill -9 31367

 mvn liquibase:generateChangeLog
 
pm2 start yarn --name "hyster-yale-frontend" -- start

sudo reboot -p


# export IP 
export NEXT_PUBLIC_BACKEND_URL=http://$(hostname -I | awk '{print $1}')/hysteryale/
