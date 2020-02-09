# Sample deploying the Djnago tutorial Polls app to AWS ECS using Docker

This is a sample to deploy [django tutorial Polls app](https://docs.djangoproject.com/en/2.2/intro/tutorial01/) to Elastic Container Service (ECS) of Amazon Web Service (AWS) .  
This repository does not include the Polls app created in the tutorial.  
See below for a detailed explanation.  

https://qiita.com/Brokenumbrella/items/2ce3fceadfaa3d62e06f  
(Sorry, this is in Japanese.)  

### Operation confirmed environment

- Ubuntu 18.04.3 LTS  
  Docker version 19.03.5, build 633a0ea838  
  docker-compose version 1.25.0, build 0a186604  

- Windows 10 Enterprise 1903 build 18362.418  
  Use Docker for Windows  
  Docker version 19.03.5, build 633a0ea  
  docker-compose version 1.24.1, build 4667896b  
  **[Note] On Windows, execute the command on Git-Bash.**  
  **PowerShell does not work because id command cannot be used.**

### Composition

- OS: Alpine3  
- Language: Python3 (based on the official Python DockerImage)  
- Framework: Django2  
- WSGI server: uwsgi  
- Web server: nginx  
- Database: mysql8  

### Installation Version

- Alpine 3.1.0  
- Python 3.7.4  
- Django 2.2.10 or more and less than 3.0  
- uwsgi 2.0.18 or more and less than 3.0  
- nginx 1.17.8  
- MySQL 8.0.19  
- mysqlclient 1.4.6 or more and less than 2.0  
