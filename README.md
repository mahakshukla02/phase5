# phase5
# CI/CD Deployment Application
# Step1:
1. Create Springboot Application
2. Running Spring Boot Application
3. OUTPUT at localhost
4. Creating Jar file by adding finalName tag in build part of pom.xml 
5. Then update Maven Project and run mvn clean install to create Jar file of project
6. In eclipse we get jar files created


# Step2:
1.Login to AWS Account:
2. Create an instance:
•	Choose EC2 as service
•	We will select AMI as Amazon Linux AMI
3.Launch Instance and download key-pair
4.Use Puttygen to create a private key
5.Launch Putty phase5
6. Install jdk 1.8 in Amazon Linux AMI:
First to go to root:  sudo su
Installing java:     yum install java-1.8.0-openjdk
7. Create an S3 Bucket in AWS to add the JAR file and make that file public
8.Upload jar file
9.Copy Object URL and make it public
10. Add the JAR file in the created amazon linux instance using the link copied from S3 Bucket:
Enter root:  sudo su
Command to add jar in this instance is: 
 wget  https://mahakphase5.s3.amazonaws.com/spring-boot-aws.jar
11. Run the JAR file using the command java -jar JARname.jar
12.Copy the Public DNS from the instance created
13.When u run this Public dns OUTPUT would be




