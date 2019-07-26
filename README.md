# Docker_tomcat
docker tomcat install  
  
downlaod Calendar.war from https://code.google.com/archive/p/gwt-examples/downloads/Calendar.war  
/home/ec2-user/tomcat/Calendar.war  
sudo docker run -it --rm -p 8080:8080 -v /home/ec2-user/tomcat/Calendar.war:/usr/local/tomcat/webapps/Calendar.war -d tomcat  
sudo docker ps  
sudo docker images  
http://35.173.251.4:8080/Calendar/Calendar.html -- working  
sudo docker stop a38236e1fed8  
sudo docker images  
sudo docker rmi tomcat  
  
#Using Dockerfile  - Dockerfile_tomcat_Cal  
sudo docker build -t tomcat_cal .  
sudo docker images  
sudo docker run -it -p 8080:8080 -d tomcat_cal  
sudo docker ps  
http://35.173.251.4:8080/Calendar/Calendar.html  -- Works  
sudo docker exec -it 676a74683172 /bin/bash  
apt-get update  
apt-get -y install vim  catalina.log  
vim /usr/local/tomcat/logs/  
