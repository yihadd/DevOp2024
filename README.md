# DevOp 2024



# Dependency
- Docker 
- Django
- Python
- git version


## Dockerfile
![1](https://github.com/user-attachments/assets/f6397274-e17b-41fb-be37-5e937413a3c4)
#### This sets the base image to Python version 3.10. The Docker image will include a Python 3.10 environment, so any Python commands and scripts can be run within the container.
![2](https://github.com/user-attachments/assets/7955e6e4-e966-43c0-b537-9c25f9f6f312)
#### This environment variable ensures that the Python output (such as print statements) is directly flushed to the console without buffering. This makes log output immediate and visible in real-time.
![3](https://github.com/user-attachments/assets/70f41dba-89df-4910-9349-4231457e0b48)
#### This sets the working directory inside the container to /code. Any subsequent commands (like file copy or execution) will take place in this directory.
![4](https://github.com/user-attachments/assets/b51a2230-4fc8-46ae-8668-b9882c01ba44)
#### This command copies the requirements.txt file from your local machine to the current working directory in the container (/code).
![5](https://github.com/user-attachments/assets/6ee16471-65d0-4740-ade4-37e97f38c715)
#### This runs the pip install command inside the container to install all dependencies listed in requirements.txt.
![6](https://github.com/user-attachments/assets/1a908c4c-c1eb-4d37-b5c3-f34d6ad2d243)
#### This copies all files from your local directory (where the Dockerfile is located) into the working directory (/code) of the container.
![7](https://github.com/user-attachments/assets/ec81f926-afda-42a3-9fe5-5c6585fe9895)
#### This tells Docker that the container will listen on port 8000, which is commonly used for Django development servers.
![8](https://github.com/user-attachments/assets/3587e989-178c-47ab-83c8-608cfce002c5)
#### This command specifies what to run when the container starts. In this case, it runs the Django development server (manage.py runserver).

# Docker Image.
![9](https://github.com/user-attachments/assets/70351c7a-3478-4b03-a2a7-53ac3bbcfdae)
1. Build the Docker images.
2. Create and start the containers.
* docker compose: use to manage multi-container docker application defind in >> docker-compose.ylm file
* ##### docker-compose.yml >> this file use to define and manage multi-container Docker application >> it allow you to describe the container, network, volumes.
* up: this start the container. if they don't exist yet, it will create them.
* --build: rebuild the image before starting.

## View the website http://127.0.0.1:8000


