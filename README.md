# Java Vulnerable Lab
This is a "Vulnerable" Web Application developed by Cyber Security and Privacy Foundation(www.cysecurity.org). This app is intended for the Java Programmers and other people who wish to learn about Web application vulnerabilities and write secure code.

## WARNING!
THIS WEB APPLICATION CONTAINS NUMEROUS SECURITY VULNERABILITIES WHICH WILL RENDER YOUR COMPUTER VERY INSECURE WHILE RUNNING! IT IS HIGHLY RECOMMENDED TO COMPLETELY DISCONNECT YOUR COMPUTER FROM ALL NETWORKS WHILE RUNNING!

### Contrast
I compile this application and use it for Contrast Scan, it is not instrumented with Assess/Protect.

# Requirements

1. Maven 3.6.3
2. Java JDK 8

## How to build and run 

### Building only
mvn compile package

### Building and running (unconfirmed)

#### Method 1.Easiest: Docker**
  The easiest way to use Java Vulnerable is using Docker which set up everything for you with 1 command line

  Steps:

     1. Install Docker: https://docs.docker.com/engine/installation/ 
     2. Install docker-compose: https://docs.docker.com/compose/install/
     3. Inside this directory, run `sudo docker-compose up` and wait untill everything is configured for you.
     4. In your Browser, go to "http://localhost:8080/JavaVulnerableLab/install.jsp
     5. Change the JDBC URL from jdbc:mysql://localhost:3306 to jdbc:mysql://mysql:3306
     6. Click the Install Button
     7. Enjoy :)

      
#### Method 2. Easy: Standalone Web Application**
  In this mehtod, you will be running an executable "JAR" file which runs the application with an embedded Apache Tomcat. 
 
    Steps:
    
        1. Install JDK
        2. Download Executable Jar from here: http://sourceforge.net/projects/javavulnerablelab/files/v0.2/JavaVulnerableLab.jar/download
        3. Double Click the JavaVulnerable.jar to run( if double click is not working, run this command "java -jar JavaVulnerable.jar" in your Terminal or CMD)
        4. In your Browser, go to "http://localhost:8080/JavaVulnerableLab/install.jsp 
        5. Click the Install Button
        
#### Method 3. Using War file (built with mvn compile package):**
  This is a NORMAL method to deploy the WAR file. 
  
  Steps:
  
       1. Install Apache Tomcat server
       2. Go to http://[Tomcat_INSTALLED_IP]:8080/manager/  (make sure you have modified tomcat-users.xml file of the tomcat to allow the manager).
       3. Download our WAR file from here: https://sourceforge.net/projects/javavulnerablelab/files/latest/JavaVulnerableLab.war/download
       4. Deploy the WAR in Apache Tomcat manager.
       5. Go to http://[Tomcat_INSTALLED_IP]:8080/JavaVulnerableLab/install.jsp 
       6. Click the Install Button
       

Get the VulnerableSpring Project from here: https://github.com/CSPF-Founder/VulnerableSpring

##### To Do 
Work on instrumentation for Assess/Protect with Docker and docker-compose. 
