# Jenkins-pipeline-project

Steps to create a full fledged Jenkins pipeline to build, test, generate test report, generate WAR file and deploy to a Tomcat server on AWS EC2 instance including sending an auto email in case the build fails-

```

1. Create an AWS EC2 instance and install the Tomcat server. Do the Port opening to access the Tomcat server.
Link to install Tomcat - https://bytesofgigabytes.com/web/how-to-install-apache-tomcat-in-aws-ec2-instance/

2. Generate a Maven project by navigating to https://start.spring.io/

3. Download and push the Maven project to a Git repository. 

4. Create a Job in Jenkins to compile the source code in Github.

5. Create a Job to test the compiled source code. Also, add post build action to publish the test report. 

6. Create a job to deploy the WAR file to a Tomcat server by entering the Tomcat credentials. Below link can be used to configure Jenkins for all three Jobs-
https://dzone.com/articles/building-a-continuous-delivery-pipeline-using-jenk

Please note user need to be added in tomcat-users.xml to allow the used to be used in Jenkins for deployment. Below link can be used to add the user-
https://www.theserverside.com/video/Step-by-step-Jenkins-Tomcat-deploy-of-a-WAR-file

```
