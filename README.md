# Docker To-Do List App

This repository contains the Docker image for the "To-Do List app."

## Docker Hub Image

You can find the Docker image on Docker Hub [here](https://hub.docker.com/repository/docker/mdfurquan313/getting-started2.0/general).

### Pulling the Docker Image

To pull the Docker image, run the following command:

```sh
docker pull mdfurquan313/getting-started2.0:tagname
```

### Running the Docker Image
To run the Docker image, execute the following command:

## Step 1: Clone the Repository
Using Git:
```sh
git clone https://github.com/MohammadFurquan/Docker_To_Do_List_app.git
```
Or download the repository as a ZIP file and extract it.

## Step 2: Navigate to the Repository Folder
Open a terminal and navigate to the folder where the repository is located:
```sh
cd Docker_To_Do_List_app/getting-started
```
## Step 3: Build the Docker Image
Run the following command to build the Docker image:
```sh
docker build -t <image_name> .
```


## Step 4: Verify the Docker Image
Check the built image using the following command:

```sh
docker image ls
```
## Step 5: Run the Docker Image
Run the following command to start the Docker image:

```sh
docker run -dp 3000:80 <image_name>
```

## Project Details
In this image, I have used two Docker images: one for the To-Do List application and one for MySQL, which I pulled from Docker Hub. I created a network between them, mounted volumes, and then composed both images.

## Docker Compose
You can use Docker Compose to run the application and the database together. Here is an example docker-compose.yml file:-
```sh
version: '3.1'

services:

  db:
    image: mysql:5.7
    volumes:
      - db_data:/var/lib/mysql
    environment:
      MYSQL_ROOT_PASSWORD: example
      MYSQL_DATABASE: todo
      MYSQL_USER: user
      MYSQL_PASSWORD: password

  app:
    image: mdfurquan313/getting-started2.0:tagname
    ports:
      - "3000:80"
    depends_on:
      - db

volumes:
  db_data:
```
## Files in this Repository
- *'Dockerfile'* : Defines the Docker image for the To-Do List application.
- *'docker-compose.yml'*: Example Docker Compose file to run the application and MySQL together.
- *'app.py'*: The application script.
- *'requirements.txt'*: Lists the Python dependencies for the application.




---
---
# Docker_To_Do_List_app
I have created docker image of "To Do List app".
 
In this image i have used two images one is of my To_Do_List application and second is of mysql which i have pulled from DockerHub 
i have created "Network" between them and "Volume Mounted" them and then i "Composed" Both the images

Here is the link of my image of Docker Hub "https://hub.docker.com/repository/docker/mdfurquan313/getting-started2.0/general" You can use this image, run a command as "docker pull mdfurquan313/getting-started2.0:tagname"
To run the image you need to run a command as "docker run -dp 3000:80 <image_id>"


If you want to download dockerfile locally download this folder "getting-started" locally 

STEP:1
Using "Git"
Downloading Zip file of this repository
STEP:2 Open Terminal in the folder of repository which you have downloaded

STEP:3 Run the following command to build docker image "docker build -t <image_name> ."

STEP:4 Now check the image by using the following command "docker image ls"

STEP:5 Run the following command to run the image "docker run -dp 3000:80 <image_id>"
