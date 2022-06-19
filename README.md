# Run-MySQL using-Docker(Term paper)

![image](https://user-images.githubusercontent.com/97139623/170854403-7cee3791-562d-4111-b070-bcb2a0e25797.png)

KULLIYYAH OF INFORMATION & COMMUNICATION TECHNOLOGY 

CSCI 3300 OPERATING SYSTEMS
 SEM 2, 2021/2022 
 
 SECTION 01
 
Group 8


#### Title:
  Tutorial to run MySQL, phpMyAdmin using-Docker
#### Name- Matric No:
1. BINTALEB AFNAN BASEM - 1826014
2. BINSHAHBAL DANYAH AHMAD SALEM - 2020600
3. HUSAM ALI AYESH QASER - 1912611
4. BAKOBAN MOHAMMAD SAID SALEH - 1813937

#### LECTURER:

Dr.RIZAL BIN MOHD. NOR

Due :
20 June 2022

---

## Table of contents
- INTRODUCTION
- SYSTEM REQUIRMENT  

<hr/>

### INTRODUCTION
Installing a relational database set with an electronic administration device is an exceptionally normal prerequisite for an extensive variety of software projects. Not too many years ago, programmers expected to download and install these parts manually into our machines to have the option to work. In any case, because of container-based technologies like docker, we can make our environment up and running in 3 simple steps.

#### Wht is Docker?
Docker is a software platform intended to make it more straightforward to make, deploy, and run applications using containers. It permits developers to bundle up an application with all the parts it needs in a container, and afterward transport it out as one package. Also, provide an image-based deployment model. This makes it easy to share an application, or set of services, with all of their dependencies across multiple environments.

This tutorial aims to get up and running a fully functional platform with MySQL Community Edition + phpMyAdmin working on your local machine with the help of docker. Let's briefly describe these elements.

MySQL Community Edition is a freely downloadable version of the world’s most popular open-source database that is supported by an active community of open source developers and enthusiasts.


---
### SYSTEM REQUIRMENT 
Operating System: Windows 11 Home

Docker Community: Docker desktop 4.9.0 

### TUTORIAL STEP-BY-STEP
1- Download Docker.(https://docs.docker.com/desktop/windows/install/);
2- Double-click InstallDocker.msi to run the installer.
![image](https://user-images.githubusercontent.com/97139623/173755705-d0858cb5-7562-4310-ba73-6fdea629ec62.png)

3- Follow the Install Wizard: accept the license, authorize the installer, and proceed with the install.
Click Finish to launch Docker.
![image](https://user-images.githubusercontent.com/97139623/173755808-abcd9b64-a228-4a0f-953e-b5b70aa8b097.png)

4- Docker starts automatically.
![image](https://user-images.githubusercontent.com/97139623/173756235-51fc950d-ad28-464b-931c-dec45a472615.png)

5- Docker loads a “Welcome” window giving you tips and access to the Docker documentation.


###  Running MySQL docker container

     - Step 1 
     Open a terminal and run the command below in order to check your docker installation
![image](https://user-images.githubusercontent.com/97139623/173756880-172f3d9e-b88d-46fe-b24d-7e8c04f2046d.png)


     - Step 2
     If you get a message like the one displayed above, it means your docker installation is ok. 
     Then you can proceed to obtain a MySQL docker image by typing the following: docker pull mysql
     and wait until the installation is completed 
   ![image](https://user-images.githubusercontent.com/97139623/174467898-231a828b-023e-45bc-b7dc-2b821bb49681.png)
   
   
 - Step 3
  so now you can run it into your local machine:
  
docker run --name ms -p 3306:3306 -e MYSQL_ROOTPASSWORD=password mysql
![image](https://user-images.githubusercontent.com/97139623/174467603-1223ef14-36e0-4721-b68c-d64c03153058.png)

- Let's explain the options for the command docker run.

The option --name allows us to assign a specific name for our running container.
The option -e is used to pass a value to the container environment variable MYSQL_ROOT_PASSWORD. 
This variable is requested by the image to run properly and it will be assigned to the root password of MySQL.


- Step 4 
Open the docker and you will see the container 
![image](https://user-images.githubusercontent.com/97139623/174467571-cd74ea26-ab61-4be4-9a25-5b55334a047a.png)

- Step 5 
open your broswer and search for (https://dev.mysql.com/downloads/workbench/)
Clik the download button 
![image](https://user-images.githubusercontent.com/97139623/174467728-8268c3fc-9e51-4478-9db9-234e1ad1e6c9.png)

choose no thanks just start my download 
![image](https://user-images.githubusercontent.com/97139623/174467759-1ebfa14c-96d1-489e-af35-1f960bae981f.png)



