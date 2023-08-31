# Docker_To_Do_List_app
 I have created docker image of "To Do List app".
 Here is the link of my image of Docker Hub "https://hub.docker.com/repository/docker/mdfurquan313/getting-started2.0/general" You can use this image, run a command as "docker pullmdfurquan313/getting-started2.0:tagname". To run the image you need to run a command as "docker run -dp 3000:80 <image_id?"

If you want to download dockerfile locally download this folder "getting-started" locally 

STEP:1
Using "Git"
Downloading Zip file of this repository
STEP:2 Open Terminal in the folder of repository which you have downloaded

STEP:3 Run the following command to build docker image "docker build -t <image_name> ."

STEP:4 Now check the image by using the following command "docker image ls"

STEP:5 Run the following command to run the image "docker run -dp 3000:80 <image_id>"
