# my RESTful web service In Java that runs in a docker container

I've created a RESTful web service In java using maven project. My data model consists of four elements which are described below:
1. Author: who created the message
2. Created: when it was created
3. Id: unique identifier to every message
4. Message: the message

It contains two get routes which are:
1. To access all the messages we use the url: http://localhost:8080/messenger/webapi/messages
2. To access messages based on the id we use the url: http://localhost:8080/messenger/webapi/messages/{id}

The data returned from the web service routes are in JSON form. The database used is a hardcoded JSON file.

To run the web service in a docker container perform the below steps:
1.
2.
3.
