                                        
                                                        Important Commands


docker history httpd. —show the history   

docker pull httpd.     —for pull the docker image

docker images.         —show all the images inside docker

docker run.     —used to create and start docker image

docker run -it.    - it is used for run in iterative way allowing you to interact with container through command line

docker run -p.    maps a host port to a container port

docker run -d. runs in background

docker run —rm automatically remove the container when it exists

docker run —name. specifies a name for the container 

docker run httpd echo “Hello World!”    in this case new conatiner will be create 

docker run —name my-container httpd echo “Hello World!” | —name option for give u to given name to conatienr 

docker run -e MY_VAR=value httpd env. | the env is execute to display the list of environmentvariable in the conatiner, 
                                   here MY_VAR is value name it can be anything

docker run -it -e MY_NAME=Abhishek ubuntu bash |. it will open the container and you can check                                                                                                                   the env variable inside it

docker run -e APP_ENV=production -e APP_VERSION=1.0 nginx

or 

docker run -d\

            -e APP_VERSION=1.0 nginx\

            -e MY_NAME=Abhishek ubuntu bash

docker ps  — show all running conatiner

docker run -it -e COLLEGE=CSE ubuntu /bin/bash

docker ps -a | list all container running/existed/stopped

docker rmi 8fevcehrjk | remove docker image

docker rmi -f <image_id> | remove the image forcefully

docker unpause <container_id/name>. | unpause a paused container

docker kill <container_id/name>.  | kill a container(force stop)

docker rm <container_id/name> | Remove a container

docker container prune. | Remove all stopped containers

                                TASK 1:-
You are a DevOps trainee and need to deploy the Apache HTTP Server (httpd) using Docker for testing a static website. Pull the Apache server image from Docker Hub, create a container named apache-web, and run it in detached mode. Map port 8081 on the host machine to port 80 inside the container so that the website can be accessed through a browser.
Tasks:
Pull the Apache (httpd) Docker image.
Verify that the image is successfully downloaded.
Run the container with the specified name and port mapping.
Check the list of running containers.
Access the Apache web server using a browser.
<img width="445" height="157" alt="Screenshot 2026-04-15 at 5 10 55 PM" src="https://github.com/user-attachments/assets/208bf7aa-a2bd-411c-b1e7-767bf15fca99" />


<img width="1033" height="339" alt="Screenshot 2026-04-15 at 5 02 51 PM" src="https://github.com/user-attachments/assets/6867aa1e-7b20-47f7-8c64-6fc290cf90f0" />

                       Task  2:
                       
Deploy a MySQL database server using Docker. Configure the container with environment variables to set the root password, create a database named college, and create a user with credentials. Run the container in detached mode and verify that the database is running successfully.

<img width="998" height="389" alt="Screenshot 2026-04-15 at 5 18 57 PM" src="https://github.com/user-attachments/assets/4f47c16f-9ac5-439a-9c90-d54ad605d17d" />




<img width="936" height="288" alt="Screenshot 2026-04-15 at 5 20 26 PM" src="https://github.com/user-attachments/assets/233de7c7-51aa-44ea-940b-7eb3dc7c0e7f" />



<img width="886" height="369" alt="Screenshot 2026-04-15 at 5 20 49 PM" src="https://github.com/user-attachments/assets/12330977-4ad2-493b-b75b-58c2e434e99b" />



                                 Task 3:-
  Run an Ubuntu container using Docker, pass an environment variable COLLEGE=CSE, verify it inside the container, and observe what happens after stopping the container.
  
<img width="1004" height="386" alt="Screenshot 2026-04-15 at 5 25 59 PM" src="https://github.com/user-attachments/assets/55b66104-50ea-47b9-84da-0af48cd7ff58" />

After resteart----------


<img width="844" height="98" alt="Screenshot 2026-04-15 at 5 28 16 PM" src="https://github.com/user-attachments/assets/a499ae7b-9474-483f-94f8-9100dc76a1bc" />



                                     Task 4:-
Run a Docker container named DB-app using the MongoDB image and expose it so that it can be accessed from the host system.


<img width="1024" height="392" alt="Screenshot 2026-04-15 at 5 33 06 PM" src="https://github.com/user-attachments/assets/3e455c35-1bc6-49e9-a80a-0849bde46d61" />


                              Task 5:-
You are a DevOps engineer in a startup company. The development team asks you to quickly deploy a simple web page that displays the message:

Use the official httpd Docker image.
Run the container so it is accessible on port 8080 of the host machine.
Create or update an HTML file inside the container to display the required message.
Verify the output using a command-line tool.
Properly stop and remove the container after testing.


<img width="528" height="227" alt="Screenshot 2026-04-15 at 5 36 08 PM" src="https://github.com/user-attachments/assets/158b5153-f42e-43e0-b7ae-a6956317e918" />



<img width="1034" height="383" alt="Screenshot 2026-04-15 at 5 35 35 PM" src="https://github.com/user-attachments/assets/dd5bd2db-84da-4a49-8aeb-fb8f53aeb021" />

                                                        Task 6:-
                                                        
  How would you use the docker run command with -it, -e, -v, and --name to:
•	Set an environment variable APP_ENV=production.	
•	Bind a local directory /app/data to /data inside the container.	
•	Name the container my_app.	


<img width="684" height="230" alt="Screenshot 2026-04-15 at 5 45 35 PM" src="https://github.com/user-attachments/assets/2f4c99a5-327e-490e-8dbb-95f6766ddcf1" />


In another terminal:---


<img width="815" height="184" alt="Screenshot 2026-04-15 at 5 45 48 PM" src="https://github.com/user-attachments/assets/c37e6abe-8232-4b30-8993-3e288141b816" />

Important Container command:---------------

Unpause a paused container 
docker unpause <container_id/name>

Kill a container (force stop) 
docker kill <container_id/name>

Remove a container 
docker rm <container_id/name>

Remove all stopped containers 
docker container prune

                                 Task 7:--
You need to start a new container using the nginx image while setting an environment variable ENV_MODE=production. Write the docker run command to achieve this.


<img width="591" height="186" alt="Screenshot 2026-04-15 at 5 55 10 PM" src="https://github.com/user-attachments/assets/4f36a205-2790-4c56-b9c5-bd70a26617e6" />


                                  Task 8:-------

								  
You are a DevOps engineer at a university. The web development team has built a simple HTML-based portal and wants it deployed using Docker.
Use the official httpd image.
Name the container college_portal.
Run it in detached mode.
Expose container port 80 to host port 8080.
Set environment variable ENV=production.
Attach a Docker volume named portaldata to store website files.
Modify the index.html file inside the container.
Verify the output in the browser.
Check logs if the page is not loading.
Stop and remove the container.
Remove the volume and image after testing.	



<img width="1065" height="394" alt="Screenshot 2026-04-15 at 6 01 10 PM" src="https://github.com/user-attachments/assets/96fb42e3-e15a-4c17-9815-90de90475928" />


<img width="544" height="181" alt="Screenshot 2026-04-15 at 6 01 30 PM" src="https://github.com/user-attachments/assets/6dfc2439-3153-4484-861e-327f82f028cd" />


																		   Unit-3

Monolithic vs Microservices
Introduction
Software architecture has evolved significantly over time:

1980s–1990s → Monolithic applications on physical servers
2000s → N-tier applications with virtualization
Present → Microservices running in containers using Docker and Kubernetes
Microservices architecture became popular because modern applications require scalability, flexibility, and faster deployment.

Monolithic Architecture
A monolithic application is built as a single unified application where all components are tightly coupled.

It mainly contains:

User Interface (UI)
Business Logic
Database Access Layer
All modules are developed and deployed together.

Example of Monolithic Application
An E-commerce application where:

Frontend
Backend
Authentication
Payment
Database
are combined into one large application.

Advantages of Monolithic Architecture
Simple deployment
Easy debugging and testing
Faster internal communication
Suitable for small applications
Disadvantages of Monolithic Architecture
Difficult to scale specific modules
Large codebase becomes hard to manage
Technology upgrades become difficult
One failure can affect entire application
Slower development for large teams
Microservices Architecture
Microservices architecture divides an application into multiple small independent services.

Each service:

Performs a specific business task
Runs independently
Communicates using APIs
Can use its own database
Example of Microservices
An online shopping platform may contain:

User Service
Product Service
Payment Service
Order Service
Recommendation Service
Each service works independently.

Advantages of Microservices
Advantage	Description
Scalability	Services can scale independently
Independent Deployment	Update one service without affecting others
Fault Isolation	Failure in one service does not stop entire system
Technology Flexibility	Different technologies can be used
Faster Development	Teams can work independently
Easier Maintenance	Small services are easier to manage
Disadvantages of Microservices
Complex architecture
Difficult service communication
More deployment management
Monitoring becomes challenging
Requires container orchestration tools
Monolithic vs Microservices
Feature	Monolithic	Microservices
Architecture	Single application	Multiple independent services
Scalability	Entire app scaled together	Individual services scaled
Deployment	Single deployment	Independent deployment
Fault Isolation	Low	High
Flexibility	Less flexible	Highly flexible
Maintenance	Difficult for large apps	Easier due to smaller services
Technology Stack	Usually single stack	Multiple stacks possible
Role of Containers in Microservices
Microservices are commonly deployed using containers such as Docker.

Benefits:

Lightweight deployment
Faster startup time
Isolation between services
Better resource utilization
Easy scalability
Kubernetes is often used to manage multiple containers.

Real-World Examples
Netflix
Amazon
Flipkart
Swiggy
Zomato
These platforms use microservices to handle millions of users efficiently.

Important Viva Questions
1. What is a monolithic application?
A monolithic application is a single unified application where all components are tightly coupled and deployed together.

2. What are microservices?
Microservices are small independent services that work together to form an application.

3. Why are microservices preferred over monolithic architecture?
Because they provide scalability, flexibility, independent deployment, and fault isolation.

4. What is fault isolation in microservices?
Failure of one service does not affect the complete application.

5. Why are containers used in microservices?
Containers provide lightweight, isolated, and portable environments for running services.

Conclusion
Monolithic architecture is simple and suitable for small applications, while microservices architecture is better for large-scale modern applications requiring scalability, flexibility, and faster deployment.

                                              Container

Containers
Introduction
Containers are lightweight virtualization technologies that allow multiple isolated applications to run on a single operating system.

Containers package:

Application code
Dependencies
Libraries
Runtime environment
This makes applications portable and consistent across different systems.

What is a Container?
A container is an isolated environment that shares the host operating system kernel while running applications independently.

Containers are widely used in DevOps and cloud computing because they are:

Lightweight
Fast
Portable
Scalable
Features of Containers
OS-level virtualization
Lightweight compared to Virtual Machines
Fast startup time
Efficient resource utilization
Portable across environments
Isolation between applications
Containers vs Virtual Machines
Feature	Containers	Virtual Machines
Virtualization Type	OS-level virtualization	Hardware-level virtualization
Size	Lightweight	Heavy
Startup Time	Seconds	Minutes
Resource Usage	Low	High
OS Requirement	Shares host kernel	Separate guest OS
Performance	Faster	Slower compared to containers
Working of Containers
Containers use:

Namespaces → for process isolation
Control Groups (cgroups) → for resource limits
Container Runtime → to run containers
The host operating system kernel is shared among all containers.

Advantages of Containers
Faster deployment
Better resource utilization
Easy scalability
Consistent development environment
Simplified application deployment
High portability
Containers and Microservices
Containers are commonly used to deploy microservices.

Each microservice can run inside its own container with:

Required dependencies
Runtime environment
Libraries
Benefits:

Independent deployment
Fault isolation
Better scalability
Faster updates
Docker and Kubernetes
Docker
Docker is a containerization platform used to:

Build containers
Run containers
Manage container images
Kubernetes
Kubernetes is a container orchestration tool used to:

Manage multiple containers
Auto-scale applications
Self-heal failed containers
Handle container networking
Real-World Uses of Containers
Containers are widely used in:

Cloud applications
CI/CD pipelines
Microservices architecture
DevOps automation
Scalable web applications
Companies using containers:

Netflix
Amazon
Google
Spotify
Important Viva Questions
1. What is a container?
A container is a lightweight isolated environment used to run applications along with their dependencies.

2. Why are containers lightweight?
Because they share the host operating system kernel instead of running a separate OS.

3. What is the difference between containers and VMs?
Containers share the host OS kernel while VMs use separate guest operating systems.

4. What is Docker?
Docker is a platform used for containerization.

5. What is Kubernetes?
Kubernetes is a container orchestration platform used to manage multiple containers.

6. Why are containers useful in microservices?
Containers provide portability, scalability, and isolation for microservices deployment.

Conclusion
Containers provide lightweight, fast, and portable application deployment environments. They are a core technology in modern DevOps and microservices architecture.


<img width="697" height="556" alt="Screenshot 2026-05-21 at 12 23 15 PM" src="https://github.com/user-attachments/assets/bba19f63-6ffc-46b8-90c9-358a8c015283" />

# Practical 01 - Docker Compose Basics

# Aim

To understand the basics of Docker Compose and deploy an Nginx container using a docker-compose.yml file.

---

# Problem Statement

Create a Docker Compose configuration file to run an Nginx web server container and verify the deployment using Docker Desktop and browser.

---

# Requirements

- Docker Desktop
- Docker Compose
- VS Code

---

# Docker Compose File

```yaml
services:
  web:
    image: nginx
    ports:
      - "8080:80"
```

---

# Explanation

## services
Defines all containers used in the application.

---

## web
Name of the service.

---

## image: nginx
Pulls official Nginx image from Docker Hub.

---

## ports
Maps host port to container port.

```text
8080 → Host Port
80 → Container Port
```

---

# Steps Performed

## Step 1: Open Project Folder

Navigate to:

```text
C:\Users\Lenovo\OneDrive\Desktop\devops2\unit3\03-Docker-Compose-Basics
```

---

## Step 2: Create docker-compose.yml

Created Docker Compose configuration file.

---

## Step 3: Run Docker Compose

Command used:

```bash
docker compose up -d
```

---

## Step 4: Verify Running Container

Command used:

```bash
docker compose ps
```

---

## Step 5: Open Browser

Visited:

```text
http://localhost:8080
```

Verified Nginx web server output.
# Result

Successfully created and deployed an Nginx container using Docker Compose.

---

# Conclusion

Docker Compose simplifies container deployment and management using a single YAML configuration file.


                                                              

<img width="779" height="445" alt="Screenshot 2026-05-21 at 12 27 46 PM" src="https://github.com/user-attachments/assets/0e307d11-d9b2-4a3b-8afc-f7020be41df3" />


# Node.js + MongoDB using Docker Compose

## Introduction

Docker Compose allows multiple containers to run together using a single YAML configuration file.

In this project:
- Node.js container acts as application service
- MongoDB container acts as database service

Both services communicate using Docker Compose networking.

---

# Services Used

## 1. Node.js Service

Used as application container.

```yaml
app:
  image: node:18
```

---

## 2. MongoDB Service

Used as database container.

```yaml
mongo:
  image: mongo:6
```

---

# Features Used

- Multi-container deployment
- Docker Compose networking
- Environment variables
- Persistent volumes
- Service dependency management

---

# Environment Variables

```yaml
environment:
  - MONGO_URL=mongodb://mongo:27017/mydb
```

Explanation:
- `mongo` is the MongoDB service name
- `27017` is MongoDB default port
- `mydb` is database name

---

# depends_on

```yaml
depends_on:
  - mongo
```

Ensures MongoDB container starts before Node.js container.

---

# Volumes

```yaml
volumes:
  - mongo-data:/data/db
```

Used for persistent MongoDB data storage.

---

# Docker Compose Networking

Docker Compose automatically creates:
- internal network
- DNS-based communication

Containers communicate using service names.

Example:

```text
mongodb://mongo:27017/mydb
```

---

# Advantages

- Easy multi-container management
- Simplified networking
- Better scalability
- Portable development environment
- Faster deployment

---

# Important Viva Questions

## 1. Why is Docker Compose used?
Docker Compose is used to manage multi-container applications.

---

## 2. What is the role of depends_on?
It controls startup order between services.

---

## 3. Why are volumes used?
Volumes provide persistent data storage.

---

## 4. How do containers communicate in Docker Compose?
Containers communicate using service names through Docker networking.

---

## 5. What is the default MongoDB port?
27017

---

# Conclusion

Docker Compose simplifies deployment and management of Node.js and MongoDB multi-container applications.

                                                          WordPress-MySql
														<img width="708" height="558" alt="Screenshot 2026-05-21 at 12 31 19 PM" src="https://github.com/user-attachments/assets/735c8650-9462-44b8-b168-32c38897c243" />

														<img width="460" height="471" alt="Screenshot 2026-05-21 at 12 32 19 PM" src="https://github.com/user-attachments/assets/c5b23234-93ab-4729-a742-7612b6326e47" />

# WordPress + MySQL using Docker Compose

## Introduction

Docker Compose is used to manage multi-container applications using a single YAML configuration file.

In this project:
- WordPress acts as frontend application
- MySQL acts as backend database

Both containers communicate through Docker networking.

---

# Services Used

## 1. WordPress Service

```yaml
wordpress:
  image: wordpress:latest
```

Runs WordPress web application.

---

## 2. MySQL Service

```yaml
db:
  image: mysql:5.7
```

Runs MySQL database server.

---

# Features Used

- Multi-container deployment
- Docker networking
- Environment variables
- Persistent volumes
- Service dependency management

---

# Environment Variables

## WordPress Configuration

```yaml
WORDPRESS_DB_HOST: db:3306
WORDPRESS_DB_USER: wpuser
WORDPRESS_DB_PASSWORD: wppass
WORDPRESS_DB_NAME: wpdb
```

Used to connect WordPress with MySQL database.

---

## MySQL Configuration

```yaml
MYSQL_DATABASE: wpdb
MYSQL_USER: wpuser
MYSQL_PASSWORD: wppass
MYSQL_ROOT_PASSWORD: rootpass
```

Used to configure MySQL database and credentials.

---

# Docker Compose Networking

Docker Compose automatically creates internal networking.

Containers communicate using:
- service names
- internal DNS

Example:

```text
db:3306
```

---

# Volumes

```yaml
volumes:
  - db-data:/var/lib/mysql
```

Provides persistent database storage.

---

# depends_on

```yaml
depends_on:
  - db
```

Ensures database container starts before WordPress container.

---

# Advantages

- Easy deployment
- Simplified configuration
- Better portability
- Persistent database storage
- Faster setup of web applications

---

# Important Viva Questions

## 1. Why is Docker Compose used?
Docker Compose is used to manage multi-container applications.

---

## 2. What is the role of environment variables?
Environment variables are used to configure services dynamically.

---

## 3. Why are volumes important?
Volumes provide persistent storage for database data.

---

## 4. How does WordPress connect to MySQL?
Using Docker internal networking and service names.

---

## 5. What is the purpose of depends_on?
It controls startup order between services.

---

# Conclusion

Docker Compose simplifies deployment and management of WordPress and MySQL multi-container applications.


                                                                       Unit-4
		Maven Introduction
What is Maven?
Apache Maven is a build automation and project management tool primarily used for Java projects.

It helps developers:

compile code
manage dependencies
run tests
package applications
deploy software
Maven uses a standard project structure and XML-based configuration file called pom.xml.

Why Build Tools Are Needed
Before Maven, developers faced many problems:

Manual compilation using javac
Dependency conflicts
Inconsistent builds
Repetitive testing and packaging tasks
Maven automates all these tasks.

Features of Maven
Dependency management
Build lifecycle management
Plugin support
Standard directory structure
Project packaging
Integration with CI/CD tools
Docker integration
Advantages of Maven
Reduces manual work
Simplifies dependency handling
Ensures consistent builds
Supports large projects
Improves project maintainability
Maven Architecture
Maven works using:

POM (Project Object Model)
Repositories
Plugins
Lifecycle phases
Maven Repositories
1. Local Repository
Stored in:

~/.m2/repository
Contains downloaded dependencies on local system.

2. Central Repository
Official Maven repository available online.

3. Remote Repository
Organization-specific repository shared across teams.

Common Maven Commands
Check Maven Version
mvn -version
Compile Project
mvn compile
Run Tests
mvn test
Package Application
mvn package
Install to Local Repository
mvn install
Important Viva Questions
1. What is Maven?
Maven is a build automation and dependency management tool for Java projects.

2. What is the purpose of Maven?
To automate project build, dependency management, testing, and deployment.

3. What is POM in Maven?
POM stands for Project Object Model and is represented using pom.xml.

4. What are Maven repositories?
Repositories store project dependencies and build artifacts.

5. What is the default local Maven repository location?
~/.m2/repository
Conclusion
Maven simplifies Java project development through build automation, dependency management, and standardized project structure.




POM Structure in Maven
What is POM?
POM stands for:

Project Object Model
It is the core configuration file in Maven projects.

The POM file is stored as:

pom.xml
Maven uses this file to:

manage dependencies
configure plugins
define project information
control build process
Basic Structure of pom.xml
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
         http://maven.apache.org/xsd/maven-4.0.0.xsd">

    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>demo-app</artifactId>
    <version>1.0-SNAPSHOT</version>

</project>
Important POM Elements
1. modelVersion
<modelVersion>4.0.0</modelVersion>
Specifies POM model version.

2. groupId
<groupId>com.example</groupId>
Identifies organization or company name.

Example:

com.google
org.apache
3. artifactId
<artifactId>demo-app</artifactId>
Represents project name.

4. version
<version>1.0-SNAPSHOT</version>
Defines project version.

SNAPSHOT
Indicates project is under development.

5. packaging
<packaging>jar</packaging>
Defines output type.

Common values:

jar
war
pom
Dependencies
Dependencies are external libraries required by the project.

Example:

<dependencies>

    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.13.2</version>
        <scope>test</scope>
    </dependency>

</dependencies>
Build Section
Used to configure plugins and build process.

Example:

<build>
    <plugins>

    </plugins>
</build>
Maven Coordinates
Every Maven project is uniquely identified using:

groupId + artifactId + version
Example:

com.example:demo-app:1.0-SNAPSHOT
Parent POM
A Parent POM provides common configuration for multiple projects.

Example:

<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>3.2.0</version>
</parent>
Advantages of POM
Centralized configuration
Easy dependency management
Build standardization
Plugin configuration
Better maintainability
Important Viva Questions
1. What is pom.xml?
It is the main Maven configuration file.

2. What is groupId?
It identifies organization or project group.

3. What is artifactId?
It identifies project name.

4. What is version in Maven?
Defines project release version.

5. What is SNAPSHOT version?
Indicates project is under development.

6. What is packaging in Maven?
Defines output format such as JAR or WAR.

7. What is Parent POM?
A Parent POM provides shared configuration across projects.

Conclusion
The POM file is the heart of Maven projects and controls dependencies, plugins, and build configuration.


Maven Lifecycle
What is Maven Lifecycle?
Maven Lifecycle is a sequence of predefined phases used to build and manage a project.

Each phase performs a specific task during project development.

Example:

compiling code
testing
packaging
deployment
Types of Maven Lifecycles
Maven provides three built-in lifecycles:

Default Lifecycle
Clean Lifecycle
Site Lifecycle
1. Default Lifecycle
Used for:

compilation
testing
packaging
deployment
This is the most commonly used lifecycle.

Important Default Lifecycle Phases
validate
Checks project correctness and verifies required information.

Command:

mvn validate
compile
Compiles source code.

Command:

mvn compile
test
Runs unit tests.

Command:

mvn test
package
Packages application into:

JAR
WAR
Command:

mvn package
verify
Checks package validity and quality.

Command:

mvn verify
install
Installs package into local Maven repository.

Command:

mvn install
Repository location:

~/.m2/repository
deploy
Deploys package to remote repository.

Command:

mvn deploy
2. Clean Lifecycle
Used to remove previously generated build files.

clean
Deletes target directory.

Command:

mvn clean
3. Site Lifecycle
Used to generate project documentation.

site
Creates project documentation website.

Command:

mvn site
Maven Lifecycle Flow
validate
   ↓
compile
   ↓
test
   ↓
package
   ↓
verify
   ↓
install
   ↓
deploy
Important Concept
When a later phase is executed, all previous phases run automatically.

Example:

mvn package
Automatically runs:

validate
compile
test
package
Target Directory
Maven stores generated files inside:

target/
Contains:

compiled classes
JAR files
reports
Advantages of Maven Lifecycle
Standardized build process
Reduced manual work
Better automation
Easy project management
CI/CD integration support
Important Viva Questions
1. What is Maven Lifecycle?
A predefined sequence of phases used to build and manage projects.

2. What are the three Maven lifecycles?
Default
Clean
Site
3. What does mvn compile do?
Compiles project source code.

4. What does mvn package do?
Packages application into JAR or WAR file.

5. What is the purpose of mvn clean?
Deletes previously generated build files.

6. Where are Maven build files stored?
Inside the target/ directory.

7. What happens when mvn install is executed?
Package is installed into local Maven repository.

Common Maven Lifecycle Commands
Clean Project
mvn clean
Compile Project
mvn compile
Run Tests
mvn test
Build JAR File
mvn package
Install Project
mvn install
Conclusion
Maven Lifecycle automates project build, testing, packaging, and deployment using predefined phases.


Dependency Management in Maven
What is Dependency Management?
Dependency management is the process of handling external libraries required by a project.

In Maven, dependencies are declared inside:

<dependencies>
</dependencies>
section of pom.xml.

Maven automatically:

downloads dependencies
manages versions
resolves dependency conflicts
Example Dependency
<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.13.2</version>
    <scope>test</scope>
</dependency>
Dependency Components
groupId
Identifies organization or library provider.

Example:

<groupId>junit</groupId>
artifactId
Represents library name.

Example:

<artifactId>junit</artifactId>
version
Specifies library version.

Example:

<version>4.13.2</version>
scope
Defines where dependency is available.

Example:

<scope>test</scope>
Dependency Scopes
1. compile
Default scope.

Available:

compile time
test time
runtime
Example:

Spring Core libraries
2. provided
Available during:

compile
test
NOT included at runtime.

Example:

Servlet API provided by Tomcat
3. runtime
Required only during runtime.

Example:

JDBC drivers
4. test
Available only during testing.

Example:

JUnit
Mockito
5. system
Uses local system JAR path.

Not recommended.

Transitive Dependencies
Maven automatically downloads dependencies required by other dependencies.

Example:

Project → Spring Boot → Logging Libraries
No need to manually add all libraries.

Dependency Conflict
Sometimes multiple versions of same library exist.

Example:

Library A → log4j 1.0
Library B → log4j 2.0
This creates version conflict.

Conflict Resolution
Maven uses:

Nearest Definition Wins
Nearest dependency in dependency tree is selected.

Excluding Dependencies
Unwanted dependencies can be removed using:

<exclusions>
    <exclusion>
        <groupId>com.example</groupId>
        <artifactId>old-lib</artifactId>
    </exclusion>
</exclusions>
Dependency Management Section
Used to centrally manage dependency versions.

Example:

<dependencyManagement>
    <dependencies>

    </dependencies>
</dependencyManagement>
Advantages of Dependency Management
Automatic dependency download
Reduced manual work
Better version control
Easy project maintenance
Faster project setup
Important Viva Questions
1. What is dependency management in Maven?
Dependency management handles external libraries required by a project.

2. Where are dependencies declared?
Inside pom.xml.

3. What is dependency scope?
It defines where a dependency is available.

4. What are transitive dependencies?
Dependencies automatically downloaded by Maven for other dependencies.

5. What is dependency conflict?
When multiple versions of same library exist.

6. How does Maven resolve dependency conflicts?
Using nearest definition wins strategy.

7. What is the purpose of exclusions?
To remove unwanted transitive dependencies.

Common Dependency Commands
Download Dependencies
mvn dependency:resolve
View Dependency Tree
mvn dependency:tree
Clean and Install
mvn clean install
Conclusion
Maven dependency management simplifies handling of external libraries and automatically resolves dependencies and version conflicts.


Maven Plugins
What are Maven Plugins?
Maven plugins are components that perform specific tasks during the build lifecycle.

Examples:

compiling code
running tests
packaging applications
creating JAR files
Docker integration
Maven functionality is mostly implemented through plugins.

Plugin Structure
Plugins are configured inside:

<build>
    <plugins>

    </plugins>
</build>
section of pom.xml.

Plugin Components
groupId
Identifies plugin organization.

artifactId
Specifies plugin name.

version
Defines plugin version.

Maven Compiler Plugin
Used to compile Java source code.

Example:

<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-compiler-plugin</artifactId>

    <configuration>
        <source>17</source>
        <target>17</target>
    </configuration>

</plugin>
Purpose of Compiler Plugin
Compiles Java code
Defines Java version
Generates .class files
Maven Surefire Plugin
Used to run unit tests.

Example:

<plugin>
    <artifactId>maven-surefire-plugin</artifactId>
    <version>3.1.2</version>
</plugin>
Purpose of Surefire Plugin
Executes test cases
Generates test reports
Supports JUnit testing
Maven Shade Plugin
Used to create:

Uber JAR / Fat JAR
An Uber JAR contains:

project code
all dependencies
executable configuration
inside a single JAR file.

Shade Plugin Example
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-shade-plugin</artifactId>
    <version>3.5.0</version>
</plugin>
Advantages of Uber JAR
Easy deployment
Portable execution
Single executable file
Simplified dependency handling
Maven Wrapper (mvnw)
Maven Wrapper ensures consistent Maven version across all systems.

Files created:

mvnw
mvnw.cmd
.mvn/
Generate Maven Wrapper
Command:

mvn wrapper:wrapper
Using Maven Wrapper
Linux/macOS:

./mvnw clean package
Windows:

mvnw.cmd clean package
Docker Maven Plugin
Used for Docker integration with Maven.

Example:

<plugin>
    <groupId>com.spotify</groupId>
    <artifactId>dockerfile-maven-plugin</artifactId>
    <version>1.4.13</version>
</plugin>
Advantages of Maven Plugins
Build automation
Test automation
Packaging support
Docker integration
CI/CD compatibility
Important Viva Questions
1. What are Maven plugins?
Plugins are components that perform specific build tasks.

2. What is the purpose of Maven Compiler Plugin?
To compile Java source code.

3. What is Maven Surefire Plugin used for?
To execute unit tests.

4. What is an Uber JAR?
A single executable JAR containing application code and dependencies.

5. What is the purpose of Maven Wrapper?
To maintain consistent Maven version across environments.

6. Which plugin is used for Docker integration?
dockerfile-maven-plugin

Common Plugin Commands
Compile Project
mvn compile
Run Tests
mvn test
Package Application
mvn package
Create Wrapper
mvn wrapper:wrapper
Conclusion
Maven plugins automate compilation, testing, packaging, and Docker integration during the build lifecycle.

Maven - Build Automation and Project Management
This unit covers Apache Maven, a powerful build automation tool and project management framework for Java projects.

Topics Covered
Maven Introduction - What is Maven and why use it
POM Structure - Understanding the Project Object Model
Maven Lifecycle - Build phases and goals
Dependency Management - Managing project dependencies
Maven Plugins - Extending Maven functionality
Maven Docker Integration - Containerizing Maven projects
Learning Outcomes
Understand Maven architecture and principles
Create and configure Maven projects
Manage project dependencies effectively
Use Maven lifecycle for build automation
Integrate Maven with Docker
Build reproducible and portable Java applications
Directory Structure
01-Maven-Introduction/ - Getting started with Maven
02-POM-Structure/ - Understanding pom.xml
03-Maven-Lifecycle/ - Build phases and goals
04-Dependency-Management/ - Managing dependencies
05-Maven-Plugins/ - Using and configuring plugins
06-Maven-Docker-Integration/ - Docker integration examples
practice-questions.md - Review questions and exercises




Practice Questions and Exercises
Basic Concepts
Question 1: Maven Fundamentals
Q: What is Apache Maven and what are its three main advantages over traditional build systems?

A: Apache Maven is a build automation tool and project management framework for Java projects. Three main advantages are:

Convention over Configuration - Uses sensible defaults, reducing configuration needed
Automatic Dependency Management - Handles project dependencies automatically
Consistent Build Process - Provides standardized project structure across teams
Question 2: Maven Coordinates
Q: Identify the three coordinates in the following Maven dependency:

com.google.guava:guava:31.0.1-jre
A:

GroupId: com.google.guava
ArtifactId: guava
Version: 31.0.1-jre
POM Structure
Question 3: POM Elements
Q: What does POM stand for and list 5 essential sections in a pom.xml file.

A: POM stands for Project Object Model. Five essential sections are:

<modelVersion> - POM version
<groupId>, <artifactId>, <version> - Project identification
<dependencies> - External libraries
<properties> - Reusable values
<build> - Build configuration
Question 4: POM Inheritance
Q: What is a parent POM and how does it benefit multi-module projects?

A: A parent POM is a common pom.xml file that contains shared configuration, dependencies, and properties. Benefits:

Eliminates duplicate configuration
Ensures consistent versions across modules
Simplifies dependency management
Facilitates consistent build process
Maven Lifecycle
Question 5: Build Phases
Q: List the 7 main phases of Maven's default lifecycle in order.

A:

validate
compile
test
package
verify
install
deploy
Question 6: Maven Commands
Q: What command would you use to clean the project, run all tests, and package without deploying?

A: mvn clean test package

Question 7: Skip Tests
Q: How would you build a Maven project while skipping all tests?

A: Use one of these approaches:

mvn clean package -DskipTests
mvn clean package -Dmaven.test.skip=true
Dependency Management
Question 8: Dependency Scopes
Q: Match each scope with its description:

Scope	Description
compile	Only needed for test compilation and execution
test	Available in all classpaths
provided	Not needed for compilation, only at runtime
runtime	Expected to be provided by JDK or runtime
A:

compile → Available in all classpaths
test → Only needed for test compilation and execution
provided → Expected to be provided by JDK or runtime
runtime → Not needed for compilation, only at runtime
Question 9: Transitive Dependencies
Q: What are transitive dependencies and why are they important in Maven?

A: Transitive dependencies are dependencies that your project's dependencies depend on. They're important because:

Maven automatically manages them
Reduces configuration overhead
Helps prevent version conflicts
Ensures all required libraries are available
Question 10: Dependency Tree
Q: What Maven command would you use to view all dependencies including transitive ones?

A: mvn dependency:tree

Maven Plugins
Question 11: Plugins vs. Plugins Goals
Q: Explain the difference between a Maven plugin and a plugin goal.

A:

Plugin: A software component that provides reusable goals (e.g., maven-compiler-plugin)
Goal: A specific task executed by a plugin (e.g., compile goal of compiler plugin)
Question 12: Plugin Configuration
Q: Write a Maven plugin configuration to set Java compilation source and target to version 11.

A:

<plugin>
  <groupId>org.apache.maven.plugins</groupId>
  <artifactId>maven-compiler-plugin</artifactId>
  <version>3.8.1</version>
  <configuration>
    <source>11</source>
    <target>11</target>
  </configuration>
</plugin>
Maven Docker Integration
Question 13: Multi-stage Docker Build
Q: What are the benefits of using a multi-stage Docker build for Java applications?

A: Benefits include:

Smaller final image size (build dependencies excluded)
Faster deployment (only runtime needed)
Enhanced security (no build tools in production)
Cleaner separation of concerns
More efficient use of Docker layers
Question 14: Build Process
Q: Describe the typical workflow to build and containerize a Java application using Maven and Docker.

A:

Write source code and pom.xml
Run mvn clean package to build JAR/WAR
Create Dockerfile with appropriate base image
Build Docker image: docker build -t app:1.0 .
Test container: docker run -p 8080:8080 app:1.0
Push to registry (optional): docker push registry/app:1.0
Question 15: Maven Plugin for Docker
Q: Name two Maven plugins that can automatically build Docker images and describe one.

A:

Spotify Docker Maven Plugin - Allows building Docker images from Maven using plugin configuration
Google Jib Maven Plugin - Builds optimized Docker images without requiring a Docker daemon
Hands-on Exercises
Exercise 1: Create and Build a Maven Project
Create a Maven project from scratch with:

GroupId: org.mycompany
ArtifactId: hello-app
Version: 2.0.0
Add JUnit dependency for testing
Build the project and verify the JAR is created
Exercise 2: Dependency Management
Create a pom.xml with multiple Spring Boot dependencies
Run mvn dependency:tree to view the dependency tree
Identify and exclude an unnecessary transitive dependency
Verify the exclusion works
Exercise 3: Maven Plugins
Configure the following plugins in a pom.xml:

Maven Compiler Plugin (Java 11)
Maven JAR Plugin (with main class specified)
Maven Assembly Plugin (create fat JAR)
Build the project and verify all artifacts are created.

Exercise 4: Docker Integration
Create a Spring Boot application using Maven
Write a multi-stage Dockerfile
Build the Docker image
Run the container and verify it works
Push to a Docker registry (Docker Hub or private)
Advanced Questions
Question 16: Version Management
Q: How would you manage consistent versions across multiple dependencies in a pom.xml?

A: Use properties:

<properties>
  <spring.version>5.3.9</spring.version>
</properties>

<dependency>
  <groupId>org.springframework</groupId>
  <artifactId>spring-core</artifactId>
  <version>${spring.version}</version>
</dependency>
Question 17: Repository Configuration
Q: How do you configure a private Maven repository in pom.xml?

A:

<repositories>
  <repository>
    <id>private-repo</id>
    <url>https://nexus.example.com/repository/maven-releases/</url>
    <credentials>
      <username>user</username>
      <password>password</password>
    </credentials>
  </repository>
</repositories>
Question 18: Continuous Integration
Q: How would you set up a Maven project for CI/CD pipeline?

A:

Use consistent pom.xml versioning
Configure automated tests in Maven
Use Maven profiles for different environments
Implement dependency management
Set up automated builds on code push
Configure automated Docker image creation
Push artifacts to repository automatically
Answer Key Summary
Key Concepts to Remember:

Maven follows Convention over Configuration
Dependencies are managed through pom.xml
Build lifecycle has 7 main phases
Plugins extend Maven functionality
Docker integrates with Maven for containerization
Use properties for version management
Parent POMs reduce configuration duplication
Transitive dependencies are automatically managed
Common Commands:

mvn clean package          # Build project
mvn dependency:tree        # View dependencies
mvn clean install          # Build and install
mvn test                   # Run tests only
mvn help:describe          # Get plugin help


Introduction to GitHub Actions
What is GitHub Actions?
GitHub Actions is a CI/CD (Continuous Integration / Continuous Deployment) platform provided by GitHub.

It helps automate software workflows directly inside a GitHub repository.

Using GitHub Actions, developers can:

Build applications
Run tests
Deploy applications
Automate repetitive tasks
GitHub Actions workflows are written using YAML files. :contentReference[oaicite:0]{index=0}

What is CI/CD?
Continuous Integration (CI)
Continuous Integration means automatically:

building code
testing code
validating changes
whenever developers push code.

Example:

Developer pushes code → automatic build → automatic tests.

Continuous Deployment (CD)
Continuous Deployment means automatically deploying applications after successful build and testing.

Example:

Code Push → Build → Test → Deploy.

Why Use GitHub Actions?
Advantages:

Integrated with GitHub
Supports CI/CD automation
Easy workflow configuration
Supports Docker, Maven, NodeJS, Python, Java
Cross-platform runners
Workflow Automation
A workflow is an automated process.

Workflow files are:

written in YAML
stored inside:
.github/workflows/
A workflow contains:

Events
Jobs
Steps
Actions
Example structure from lecture notes: :contentReference[oaicite:1]{index=1}

name: My First Workflow

on: push

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Code
        uses: actions/checkout@v3

      - name: Run Script
        run: echo "Hello World"
Components of GitHub Actions
1. Events
Events decide when workflow starts.

Examples:

push
pull_request
schedule
workflow_dispatch
2. Jobs
Jobs define what work will be done.

A workflow may contain multiple jobs.

Jobs run in parallel by default.

Example:

jobs:
  build:
  test:
3. Steps
Steps define how a job executes.

Each job contains sequential steps.

Example:

steps:
  - name: Hello
    run: echo "Hello World"
4. Actions
Actions are reusable workflow components.

Example:

uses: actions/checkout@v4
5. Runners
Runners execute workflows.

Types:

GitHub-hosted runners
Self-hosted runners
GitHub supports:

Ubuntu
Windows
macOS :contentReference[oaicite:2]{index=2}
Basic Workflow Example
name: First CI Workflow

on: push

jobs:
  build:

    runs-on: ubuntu-latest

    steps:

      - uses: actions/checkout@v4

      - name: Print Message
        run: echo "GitHub Actions Working Successfully"
Important Viva Questions
What is GitHub Actions?
GitHub Actions is a CI/CD automation platform integrated with GitHub.

Where are workflow files stored?
.github/workflows/
Which language is used to define workflows?
YAML.

What is a runner?
A server that executes GitHub Actions workflows.

Difference between CI and CD?
CI → automatic build/testing.

CD → automatic deployment.

Conclusion
GitHub Actions automates software workflows using YAML-based pipelines and supports CI/CD directly inside GitHub repositories.


Workflow Triggers
What are Workflow Triggers?
Workflow triggers decide when a GitHub Actions workflow should run.

Triggers are defined using the:

on:
keyword inside workflow files. :contentReference[oaicite:0]{index=0}

Common Workflow Triggers
1. Push Trigger
Runs workflow whenever code is pushed to repository.

Example:

on:
  push:
Specific branch:

on:
  push:
    branches:
      - main
Use case:

automatic builds
automatic testing
CI pipelines
2. Pull Request Trigger
Runs workflow when a pull request is created or updated.

Example:

on:
  pull_request:
Specific branch:

on:
  pull_request:
    branches:
      - main
Use case:

validate code before merging
run tests on PRs
3. Schedule Trigger
Runs workflow automatically at scheduled times.

Uses cron syntax.

Example:

on:
  schedule:
    - cron: '0 0 * * *'
Example meaning:

Runs every day at midnight.

Use case:

backup jobs
scheduled testing
maintenance tasks
4. Manual Workflow Trigger
Allows workflows to be started manually.

Keyword:

workflow_dispatch
Example:

on:
  workflow_dispatch:
Use case:

manual deployments
on-demand builds
debugging pipelines
Multiple Triggers
GitHub Actions supports multiple triggers.

Example:

on:
  push:
    branches:
      - main

  pull_request:
    branches:
      - main
Workflow runs for:

push events
pull request events
Trigger Example
name: CI Workflow

on:
  push:
    branches:
      - main

jobs:

  build:

    runs-on: ubuntu-latest

    steps:

      - name: Hello
        run: echo "Workflow Triggered Successfully"
Trigger Use Cases
Trigger	Purpose
push	Run build after code push
pull_request	Validate pull requests
schedule	Timed automation
workflow_dispatch	Manual execution
Important Viva Questions
What is a workflow trigger?
An event that starts a GitHub Actions workflow.

Which keyword defines triggers?
on:
Which trigger is used for manual execution?
workflow_dispatch
Which trigger uses cron expressions?
schedule
Which trigger runs after pushing code?
push
Conclusion
Workflow triggers control when GitHub Actions workflows execute using events such as push, pull_request, schedule, and manual execution.


Jobs, Steps, Actions and Runners
Key Components of GitHub Actions
GitHub Actions workflows are built using several important components:

Jobs
Steps
Actions
Runners
These components define how automation workflows execute. :contentReference[oaicite:0]{index=0}

1. Jobs
A job is a group of tasks executed inside a workflow.

Each workflow can contain one or multiple jobs.

Example:

jobs:
  build:
  test:
Characteristics:

Jobs run independently.
Jobs run in parallel by default.
Jobs can depend on other jobs.
Job Example
jobs:

  build:

    runs-on: ubuntu-latest

    steps:
      - run: echo "Building Application"
Job Dependencies
Jobs can wait for another job using:

needs:
Example:

jobs:

  build:
    runs-on: ubuntu-latest

  deploy:
    needs: build
    runs-on: ubuntu-latest
Here:

Build job executes first.
Deploy job runs after build completes.
2. Steps
Steps define individual commands executed inside a job.

Each job contains one or more steps.

Example:

steps:
  - name: Print Message
    run: echo "Hello GitHub Actions"
Characteristics:

Steps run sequentially.
Each step performs one task.
Can use commands or reusable actions.
Step Example
steps:

  - name: Install Dependencies
    run: npm install

  - name: Run Tests
    run: npm test
3. Actions
Actions are reusable workflow components.

Instead of writing everything manually, predefined actions can be used.

Syntax:

uses:
Example:

uses: actions/checkout@v4
Popular actions:

Action	Purpose
actions/checkout	Clone repository
actions/setup-java	Configure Java
actions/cache	Dependency caching
upload-artifact	Store build files
Example Action
steps:

  - name: Checkout Code
    uses: actions/checkout@v4
Purpose:

Downloads repository source code.

4. Runners
Runners are machines that execute workflows.

Each job requires a runner.

Defined using:

runs-on:
Example:

runs-on: ubuntu-latest
Types of Runners
GitHub Hosted Runner
Managed by GitHub.

Supported environments:

Ubuntu
Windows
macOS
Example:

runs-on: ubuntu-latest
Self Hosted Runner
Managed by user or organization.

Used for:

custom hardware
internal environments
private infrastructure
Complete Example
name: Example Workflow

on:
  push:

jobs:

  build:

    runs-on: ubuntu-latest

    steps:

      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Print Message
        run: echo "Workflow Running Successfully"
Important Viva Questions
What is a job?
A group of tasks executed inside a workflow.

What are steps?
Individual instructions executed inside a job.

What is an action?
Reusable workflow component used inside steps.

What does actions/checkout@v4 do?
Clones repository code into workflow environment.

What is a runner?
Machine that executes GitHub Actions workflows.

Difference between GitHub-hosted and self-hosted runners?
GitHub-hosted → managed by GitHub.

Self-hosted → managed by user.

Conclusion
Jobs, steps, actions, and runners are core building blocks of GitHub Actions workflows and together automate CI/CD pipelines.


Docker GitHub Actions Integration
What is Docker GitHub Actions Integration?
Docker can be integrated with GitHub Actions to automate:

Docker image building
Docker image testing
Container execution
CI/CD pipelines
Whenever code is pushed, GitHub Actions can automatically run Docker workflows. :contentReference[oaicite:0]{index=0}

Workflow Objective
In this workflow:

Checkout repository code
Build Docker image
Verify image creation
This demonstrates a basic CI pipeline using Docker and GitHub Actions.

Project Structure
Example structure:

repository/
│
├── app.py
├── requirements.txt
├── Dockerfile
│
└── .github/
    └── workflows/
        └── ci-cd.yml
Application File
Example Flask application:

from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello from Docker CI/CD!"

if __name__ == "__main__":
    app.run(host='0.0.0.0', port=5000)
Example adapted from practical sheet. :contentReference[oaicite:1]{index=1}

Dockerfile
Example Dockerfile:

FROM python:3.9-slim

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

CMD ["python","app.py"]
GitHub Actions Workflow
Workflow file location:

.github/workflows/ci-cd.yml
Example workflow:

name: CI-CD Pipeline

on:
  push:
    branches:
      - main

jobs:

  build:

    runs-on: ubuntu-latest

    steps:

      - name: Checkout Code
        uses: actions/checkout@v4

      - name: Build Docker Image
        run: docker build -t my-docker-app .

      - name: List Docker Images
        run: docker images
Adapted from practical document. :contentReference[oaicite:2]{index=2}

Workflow Explanation
Trigger
on:
  push:
Runs workflow when code is pushed.

Checkout Step
uses: actions/checkout@v4
Downloads repository code.

Docker Build Step
docker build
Creates Docker image.

Docker Images Step
docker images
Lists available images.

Advantages
Automated builds
Continuous integration
Faster validation
Docker workflow automation
Better deployment readiness
Important Viva Questions
Why integrate Docker with GitHub Actions?
To automate Docker build and CI/CD pipelines.

Which command builds Docker image?
docker build -t image-name .
What does actions/checkout do?
Downloads repository source code.

Where are workflow files stored?
.github/workflows/
Which event triggers this workflow?
push
Conclusion
Docker GitHub Actions integration automates container build workflows and supports continuous integration pipelines.Docker GitHub Actions Integration
What is Docker GitHub Actions Integration?
Docker can be integrated with GitHub Actions to automate:

Docker image building
Docker image testing
Container execution
CI/CD pipelines
Whenever code is pushed, GitHub Actions can automatically run Docker workflows. :contentReference[oaicite:0]{index=0}

Workflow Objective
In this workflow:

Checkout repository code
Build Docker image
Verify image creation
This demonstrates a basic CI pipeline using Docker and GitHub Actions.

Project Structure
Example structure:

repository/
│
├── app.py
├── requirements.txt
├── Dockerfile
│
└── .github/
    └── workflows/
        └── ci-cd.yml
Application File
Example Flask application:

from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello from Docker CI/CD!"

if __name__ == "__main__":
    app.run(host='0.0.0.0', port=5000)
Example adapted from practical sheet. :contentReference[oaicite:1]{index=1}

Dockerfile
Example Dockerfile:

FROM python:3.9-slim

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

CMD ["python","app.py"]
GitHub Actions Workflow
Workflow file location:

.github/workflows/ci-cd.yml
Example workflow:

name: CI-CD Pipeline

on:
  push:
    branches:
      - main

jobs:

  build:

    runs-on: ubuntu-latest

    steps:

      - name: Checkout Code
        uses: actions/checkout@v4

      - name: Build Docker Image
        run: docker build -t my-docker-app .

      - name: List Docker Images
        run: docker images
Adapted from practical document. :contentReference[oaicite:2]{index=2}

Workflow Explanation
Trigger
on:
  push:
Runs workflow when code is pushed.

Checkout Step
uses: actions/checkout@v4
Downloads repository code.

Docker Build Step
docker build
Creates Docker image.

Docker Images Step
docker images
Lists available images.

Advantages
Automated builds
Continuous integration
Faster validation
Docker workflow automation
Better deployment readiness
Important Viva Questions
Why integrate Docker with GitHub Actions?
To automate Docker build and CI/CD pipelines.

Which command builds Docker image?
docker build -t image-name .
What does actions/checkout do?
Downloads repository source code.

Where are workflow files stored?
.github/workflows/
Which event triggers this workflow?
push
Conclusion
Docker GitHub Actions integration automates container build workflows and supports continuous integration pipelines.



<img width="703" height="359" alt="Screenshot 2026-05-21 at 12 41 48 PM" src="https://github.com/user-attachments/assets/f9068782-6424-4abe-9802-6c0b21b62eb0" />
Dockerfile

<img width="407" height="152" alt="Screenshot 2026-05-21 at 12 42 38 PM" src="https://github.com/user-attachments/assets/9203b979-46e9-48e6-a41e-a7c03833de7e" />
app.py


<img width="518" height="165" alt="Screenshot 2026-05-21 at 12 45 04 PM" src="https://github.com/user-attachments/assets/00370f55-d0c7-4c34-89e7-a6cfe9247b56" />


<img width="503" height="366" alt="Screenshot 2026-05-21 at 12 46 02 PM" src="https://github.com/user-attachments/assets/69ae5935-bdf1-4657-8a16-3f55302b647b" />

<img width="896" height="488" alt="Screenshot 2026-05-21 at 12 46 38 PM" src="https://github.com/user-attachments/assets/5681ffb4-5976-45df-957e-21feaa5bcc68" />




# Java Maven CI using GitHub Actions

## What is Java Maven CI?

Java Maven CI uses **GitHub Actions** to automate Java application build and testing.

Continuous Integration (CI) automatically:

- builds Java project
- installs dependencies
- runs tests
- creates build artifacts

whenever code changes are pushed to GitHub.

---

# Why Use Maven in CI?

Maven helps automate:

- dependency management
- project compilation
- testing
- packaging

Common Maven commands:

```bash
mvn clean install
mvn test
```

---

# Java CI Workflow Components

A Java Maven workflow usually contains:

1. Checkout Repository
2. Setup JDK
3. Cache Maven Dependencies
4. Build Application
5. Run Tests
6. Upload Build Artifacts

These steps are commonly used in CI pipelines. :contentReference[oaicite:1]{index=1}

---

# Example Workflow

Example `ci.yml`:

```yaml
name: Java CI with Maven

on:
  push:
    branches:
      - main

jobs:

  build:

    runs-on: ubuntu-latest

    steps:

      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Setup Java
        uses: actions/setup-java@v4
        with:
          java-version: '21'
          distribution: 'temurin'

      - name: Build Project
        run: mvn clean install
```

---

# Setup Java Step

GitHub Actions uses:

```yaml
actions/setup-java
```

Example:

```yaml
uses: actions/setup-java@v4
```

Purpose:

- install JDK
- configure Java environment

---

# Maven Build Step

Command:

```bash
mvn clean install
```

Purpose:

- clean old builds
- download dependencies
- compile source code
- execute tests
- package application

---

# Run Tests

Command:

```bash
mvn test
```

Purpose:

Executes unit tests.

---

# Upload Artifacts

GitHub Actions can store build outputs.

Action:

```yaml
actions/upload-artifact
```

Example:

```yaml
- name: Upload Artifact
  uses: actions/upload-artifact@v4
```

---

# Advantages

- Automated Java builds
- Faster testing
- Consistent CI process
- Dependency automation
- Artifact storage

---

# Important Viva Questions

## What is Java Maven CI?

Automated Java build and testing pipeline using Maven and GitHub Actions.

---

## Which action installs Java?

```yaml
actions/setup-java
```

---

## Which Maven command executes tests?

```bash
mvn test
```

---

## What does `mvn clean install` do?

Compiles, tests, packages, and installs project.

---

## What is artifact upload?

Saving generated build files for later download or deployment.

---

# Conclusion

Java Maven CI automates Java project building, testing, and artifact generation using GitHub Actions workflows.



Practical 01 — Docker + GitHub Actions CI/CD Pipeline
Aim
To create a Dockerized Python Flask application and automate its build process using GitHub Actions Continuous Integration (CI).

Problem Statement
Build a simple Flask application using Docker and configure GitHub Actions workflow to automatically build the Docker image whenever code is pushed to GitHub repository.

Solution
Step 1 — Create Flask Application
Created a simple Python Flask web application.

app.py

from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello from Docker CI/CD!"

if __name__ == "__main__":
    app.run(host='0.0.0.0', port=5000)
Step 2 — Create Requirements File
requirements.txt

Flask
Step 3 — Create Dockerfile
Created Dockerfile for containerizing the Flask application.

FROM python:3.9-slim

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

CMD ["python","app.py"]
Step 4 — Build Docker Image
Command used:

docker build --no-cache -t my-docker-app .
Step 5 — Run Docker Container
Command used:

docker run -p 5000:5000 my-docker-app
Output:

Running on http://127.0.0.1:5000
Browser Output:

Hello from Docker CI/CD!
Step 6 — Create GitHub Actions Workflow
Created workflow file:

.github/workflows/ci-cd.yml
Workflow automatically runs on every push to GitHub.

ci-cd.yml

name: CI-CD Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Code
        uses: actions/checkout@v4

      - name: Build Docker Image
        run: docker build -t my-docker-app .
Step 7 — Push Project to GitHub
Commands used:

git init
git add .
git commit -m "Add Docker GitHub Actions workflow"
git branch -M main
git remote add origin https://github.com/AsthaMaurya05/my-docker-app.git
git push -u origin main
Step 8 — Verify GitHub Actions Workflow
After pushing code:

Workflow triggered automatically.
GitHub Actions pipeline executed successfully.
Docker image build completed successfully.


                                                                  unit-6







