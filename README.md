# DevOpsCase

This repository contains application written in python language. It also includes Dockerfile and docker-compose.yml to run the application using container.

The packages that required for the application are in the requirements.txt file and the installation is done by referencing this file.

In order to run the application in your local; Mysql, Python, Docker Engine and Docker Compose must be installed.

To test your development, after cloning the project in your local you need to run the following command in the folder;

docker-compose up --build

In this way, the image named devopscase will be created and you will have the container created from this image, and the container will remain clearly visible on your terminal screen.

If you use the command below, the container will continue to run in the background;

docker-compose up --build -d

The application connects to MySQL with environment variables. Therefore, the values of the variables specified below in the Application.py file should be added as environment variable.

'MYSQL_USERNAME'
'MYSQL_PASSWORD'
'MYSQL_INSTANCE_NAME'
'MYSQL_PORT_3306_TCP_ADDR'
'MYSQL_PORT_3306_TCP_PORT'

For example, the adding command is as follows;
  export MYSQL_USERNAME='username'
