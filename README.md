<h1 align="center" id="title">VPROFILE project</h1>

<p align="center"><img src="https://socialify.git.ci/debasishdtt/vprofile-project/image?name=1&amp;owner=1&amp;theme=Light" alt="project-image"></p>

## 🌐 Project Overview
<p>In this web application project users will access the system via a browser or app by specifying the load balancer's IP address. 
  The load balancer powered by Nginx will route incoming requests to an Apache Tomcat server which is a popular choice for hosting Java web applications. 
  The user-created program is hosted on the Tomcat server with NFS servers providing optional external storage support. A MySQL database service stores user 
  login information where Memcached serves the caching purpose and a dummy RabbitMQ service (a message broker) is supplied for practice and possible 
  future connection with functional services simplifying data streaming and interconnecting applications within the system.</p>
<h5>🌟About</h5>
This project was developed as part of a guided project/tutorial on Udemy by Imran Teli. It serves as a practical exercise to reinforce the concepts learned during the tutorial.

## 🎯 Project Objectives
* Set up a local development environment for a multi-service stack.
* An infrastructure as code that can be simply deployed and reused using Vagrant and scripting.
* Set up real-world projects locally and automatically for extensive R&D.

## 💻 Built with
* Hypervisor: Oracle VM Virtual Box
* Automation: Vagrant
* Command Line Tool: Git Bash
* IDE (Optional): Visual Studio Code.

## 📚 Prerequisites
* JDK 11
* Maven 3 or later
* MySQL 5.6 or later

## 🔧 Technologies
* Spring MVC
* Spring Security
* Spring Data JPA
* Maven
* JSP
* MySQL

## 🏛️ Architectural Design
* Load Balancer: Nginx is employed to handle load balancing, efficiently routing incoming requests to our Apache Tomcat server.

* Web Server: Apache Tomcat, a popular Java web application service, hosts the developer's application.

* Database Caching: Memcached for a distributed caching system for speeding up dynamic web applications.

* Database: MySQL database service is used to store user login details securely.

* Message Broker: A dummy RabbitMQ service is included in this project, though non-functional, to introduce complexity and provide practice for future integration.

![application stack](https://github.com/debasishdtt/vprofile-project/assets/81139107/37d494c3-6ec8-4864-b0fd-564936fc9eff)
<p align="center">Fig. 1: Architectural design of the setup</p>

<h3>Flow of Execution</h3>

1. Set up required tools.
2. Clone the source code.
3. Navigate to the Vagrant directory in the source code.
4. Use the Vagrantfile to bring up virtual machines manually or automatically.
5. Validate virtual machines.
6. Set up services sequentially: MySQL, Memcached, RabbitMQ, Tomcat, Nginx.
7. Build and deploy the Java application.
8. Verify the entire setup in the browser.

<h3>How to run</h3>
Here I have used MySQL DB Installation Steps for Linux ubuntu 14.04

<pre>
  Update your package index:
$ sudo apt-get update

  Install the MySQL server:
$ sudo apt-get install mysql-server
</pre>

Then look for the file :

/src/main/resources/accountsdb <br>
accountsdb.sql file is a mysql dump file and it has to be imported to mysql db server <br>
mysql -u <user_name> -p accounts < accountsdb.sql

<h4>All of the sequentially required commands will be found: vagrant/Manual_provisioning/VprofileProjectSetupWindowsAndMacIntel.pdf</h4>

https://github.com/debasishdtt/vprofile-project/assets/81139107/132753f7-8765-4a14-a9ba-e05d29864b99

<p align="center">Fig. 2: Status of the application stack</p> 

Provisioning the entire stack with only one command 'vagrant up' is just fun.

<h4>All of the scripts required for automated provisioning will be found: vagrant/Automated_provisioning</h4>

https://github.com/debasishdtt/vprofile-project/assets/81139107/c4d6c626-e516-4236-a7d5-bf2f27b2dd98

<p align="center">Fig. 3: Automated provision of the application stack</p> 

https://github.com/debasishdtt/vprofile-project/assets/81139107/884655e6-3685-44ea-8031-fbaff169c910

<p align="center">Fig. 4: Accessing from web</p> 

## 🌱 Room for Growth

This initiative establishes the groundwork for future endeavors. The primary goal is for me to build a local multi-tier web application stack that will serve as a foundation for future projects. The relevance comes from automating the setup locally, which allows for recurrent experimentation and investigation.

The project solves frequent development difficulties, such as the unwillingness to make direct modifications to real servers and the complexity of manually configuring a local environment. The proposed solution is to use infrastructure as code to automate and repeat the setup process.

To do this, I used tools such as Oracle VM Virtual Box as a hypervisor, Vagrant for automation, and Git Bash for command execution and revision control.

The architectural design incorporates services such as Nginx for load balancing, Apache Tomcat for hosting Java web applications, RabbitMQ for messaging, Memcached for database caching, and MySQL for data storage. The entire stack is organized to offer a seamless user experience from the browser to the application, which interacts with many services.

The project encourages me to comprehend the flow and functionality of this stack, while also providing a real learning experience for DevOps engineers. The automation stack, which includes Vagrant, Virtual Box, and many scripts, makes the setup more efficient and controllable.

In conclusion, the VPROFILE Project serves as a stepping stone in mastering Vagrant automation and laying the groundwork for future projects.
