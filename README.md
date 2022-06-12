
# Create and run a CI/CD pipeline for an app

This project is about the CI CD pipeline created for Building, testing packaging and deploying on servers i.e. on both Testing server and Production server
  
  
## Tools used in the project
> **Jenkins** for Creating CI/CD pipeline  
> **Ansible** To configure the servers i.e. Testing Server and Deployment server on cloud **(AWS)**  
> **Maven** is used to build the project  
> **Tomcat** To Deploy the web application
  
## About the Project  
This project check the github repository every minute so that if any change occurs it automatically pull the code and start building it. if build was successful it will automatically deployed on testing server. That means The testers can test the application at the time it is deployed on the server and give feedback to the Developer. After that It will deployed of Production server but it requires manual Authentication So that if there is any error found by the testers or developers it will not desplayed on production side.

## Jenkns pipeline
![Jenkins pipeline 1](https://github.com/gautamjha2002/DevOps_Project-2//blob/master/Jenkins_Image/jenkins-1.png)
![Jenkins pipeline 2](https://github.com/gautamjha2002/DevOps_Project-2//blob/master/Jenkins_Image/jenkins-2.png)
