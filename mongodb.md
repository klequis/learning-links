# Links
- [Thinking in Documents](https://www.mongodb.com/blog/post/thinking-documents-part-1) - excellent for those coming from a relational model.


# MongoDB Installation

The MongoDB installation documentation is excellent. Just note that they mention glibc. This is libc on ubuntu.
- [MongoDB Installation Documentation](https://docs.mongodb.com/manual/administration/install-community/)

## Ubuntu Installation

- Make sure glibc 2.23-0ubuntu5 or above is installed
- Make sure the MongoDB from the Ubuntu distribution is not installed. If it is, do a complete uninstall
- Follow steps 1 through 4 on this page
    - Be sure to use the commands for your version of Ubuntu, e.g., 16.04

## Common Commands
Start MongoDB Server
````
$ sudo service mongod start
````
Stop MongoDB Server
````
$ sudo service mongod stop
````
Restart MongoDB Server
````
$ sudo service mongod restart
````
Start mongo shell
````
$ mongo --host 127.0.0.1:27017
````
## Install MongoDB Compass
The mongodb instructions are very straight forward
- https://docs.mongodb.com/compass/current/install/

## **older** Install MongoExpress

- sudo npm install -g mongo-express
- Find the file .../mongo-express/config.default.js and make a copy as .../mongo-express/config.js
    - On Ubuntu 16.04 this file is in /usr/lib/node_modules/mongo-express
