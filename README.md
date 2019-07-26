# Docker_tomcat
docker tomcat install  
  
downlaod Calendar.war from https://code.google.com/archive/p/gwt-examples/downloads/Calendar.war  
/home/ec2-user/tomcat/Calendar.war  
sudo docker run -it --rm -p 8080:8080 -v /home/ec2-user/tomcat/Calendar.war:/usr/local/tomcat/webapps/Calendar.war -d tomcat  
sudo docker ps  
sudo docker images  
http://35.173.251.4:8080/Calendar/Calendar.html -- working  
 
