# Simple web application containerized

This is a simple web application using Python Flask. This is used in the demonstration of containerizing a simple python app.

Below are the steps required to get this working on a base linux system.

Requirements:
vs code, Docker desktop and python

1. Install all required dependencies

Python and its dependencies

$pip install flask

2. Build docker image out of Dockerfile and run container.

$docker build -t simple-webapp .

$docker images

$docker run --name webserver -p 8080:8080 simple-webapp


3. Test

Open a browser and go to URL

http://172.17.0.1:8080/
http://172.17.0.2:8080/


outputs:
<p align="center">

  <img src="/images/ss-1.png" width="600" alt="output1">
  <img src="/images/ss-2.png" width="600" alt="output2">
  
</p>