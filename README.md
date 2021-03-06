# Jenkins using Docker


1. To run Jenkins using docker we need to run through ths command
   >docker run --name Master-Jenkins -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins
   
a. where 8080 is port you can access dashboard

b. 50000 This is only necessary if you have set up one or more inbound Jenkins agents on other machines(Master-slave concept)

c. jenkins_home is docker volume to persist all Jenkins related data like jobs, key, plugins, etc so all can survive container destruction
