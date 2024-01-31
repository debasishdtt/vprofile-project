<h1 align="center" id="title">VPROFILE project</h1>

<p align="center"><img src="https://socialify.git.ci/debasishdtt/vprofile-project/image?name=1&amp;owner=1&amp;theme=Light" alt="project-image"></p>

## 🌐 Project Overview
<p>In this web application project users will access the system via a browser or app by specifying the load balancer's IP address. 
  The load balancer powered by Nginx will route incoming requests to an Apache Tomcat server which is a popular choice for hosting Java web applications. 
  The user-created program is hosted on the Tomcat server with NFS servers providing optional external storage support. A MySQL database service stores user 
  login information and a dummy RabbitMQ service (a message broker) is supplied for practice and possible 
  future connection with functional services simplifying data streaming and interconnecting applications within the system.</p>

## 🎯 Project Objectives
* Learn a stack of services provision manually.
* Learn Vagrant automation for local setups.
* Set up real-world projects locally automatically for extensive R&D.


## 💻 Built with
* Hypervisor: Oracle VM Virtual Box
* Automation: Vagrant
* Command Line Tool: Git Bash
* IDE (Optional): Visual Studio Code.

## 🏛️ Architectural Design
* Load Balancer: Nginx is employed to handle load balancing, efficiently routing incoming requests to our Apache Tomcat server.

* Web Server: Apache Tomcat, a popular Java web application service, hosts the developer's application.

* Data Storage: For applications requiring external storage, NFS servers are available, offering flexibility and scalability.

* Database: MySQL database service is used to store user login details securely.

* Message Broker: A dummy RabbitMQ service is included in this project, though non-functional, to introduce complexity and provide practice for future integration.
  
