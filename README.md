# my RESTful web service In Java that runs in a docker container

I've created a RESTful web service In java using maven project. My data model consists of four elements which are described below:
1. Author: who created the message
2. Created: when it was created
3. Id: unique identifier to every message
4. Message: the message

It contains two get routes which are:
1. To access all the messages we use the url: http://localhost:8080/messenger/webapi/messages
2. To access messages based on the id we use the url: http://localhost:8080/messenger/webapi/messages/{id}

The data returned from the web service routes are in JSON form.

To run the web service in a docker container perform the below steps:

1. make a docker image using Dockerfile then execute docker build -f Dockerfile
2. check docker images using -  docker images
3. tag the image repository using command--   docker tag <imageid> username/repositoryname
4. push the docker image using command docker push
5. create docker-compose.yml file.
6. Start the docker image using command--   docker-compose up
