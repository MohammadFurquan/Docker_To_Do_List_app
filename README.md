# Docker To-Do List App

This repository contains the Docker image for the "To-Do List app."

## Docker Hub Image

You can find the Docker image on Docker Hub [here](https://hub.docker.com/repository/docker/mdfurquan313/getting-started2.0/general).

### Pulling the Docker Image

To pull the Docker image, run the following command:

```sh
docker pull mdfurquan313/getting-started2.0:tagname
```
Replace tagname with the specific tag you want to use.

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
Replace <image_name> with the desired name for your Docker image.
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
