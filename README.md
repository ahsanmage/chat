Installation:

Running on local
Make sure you have Node.js and npm installed.

Clone git repository

$ git clone https://github.com/ahsanmage/chat.git
$ cd chat/

Install Dependencies
$ npm install
Edit configuration file in app/config/config.json with your mongodb credentials.
You need to create a database on MongoLab, then create a database user

Setup Mongodb
Run mongod -  mongod

In Mongo CLI:
Create database: 
use chatting

Create db user: 
db.createUser({user: "root", pwd: "abcd1234", roles: [{role: "readWrite", db: "chatting" }]})

Get db users: 
db.getUsers()

Check db authentication: 
db.auth('root','abcd1234')

Start the application

$ npm start

Your app should now be running on localhost:3001