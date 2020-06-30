![Git](Screenshots/1.PNG)
# Pipeline
A pipeline in a Software Engineering team is a set of automated processes that allow Developers and DevOps professionals to reliably and efficiently compile, build and deploy their code to their production compute platforms. There is no hard and fast rule stating what a pipeline should like like and the tools it must utilise, however the most common components of a pipeline are; build automation/continuous integration, test automation, and deployment automation.

A pipeline generally consists of a set of tools which are normally broken down into the following categories;

1.Source Control
2.Build tools
3.Containerisation
4.Configuration Management
5.Monitoring

# Project Explanation
In this project we are going to first make a Jenkins images using Docker file. For that our base O.S. will be centos and we are going to configure it according to our needs to start a Jenkins server on it completely.
We are downloading the Jenkins rpm from online repository and the Open JDK to run Jenkins on top of that. We  than build our image using this docker file into a full-fledged Jenkins server ready to run.
After that we are making 5 Jobs in total in Jenkins to complete our goal. Our goal is to deploy our application on webserver as soon as the developer commits the code. Depending upon the code suitable server will be launched automatically. Event the testing part will  be done by Jenkins only. It will look for 200 code on our webserver so that if any problem is noticed automatically developer will be updated with the same so that error can be corrected. We are also making a job for monitoring purposes only so our launched website never goes down and if it does again new container will be launched with it also.

## Docker File
We have used the Docker file to build our Jenkins image in order to 
