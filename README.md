Hey Yuri, that's my final website, it does not contain an admin page but it has a working database fetch and authentication.
I made the frontend and backend seperately, therefore they have to be initialized and compiled seperately

Backend is made with the routing library Express on the nodeJS framework. and is written in pure commonjs, utilizing JSON files for initialization and using MongoDB as a database. the front end is using the NPM version controller for initialization

Frontend is written in Angulart 6, TypeScript client-side rendering framework, and Jade HTML templating engine. using Karma for test running. the backend is written in pure TypeScript, and uses NPM version controller for initialization

The entire project is written in Fedora linux distro, version 27

To run the website, you have to make sure NodeJS is installed alongside with NPM. and MongoDB is installed and running

To install MongoDB, refer to the next website and follow to guide related to your OS
https://docs.mongodb.com/manual/installation/

To install NPM and NodeJS, refer to this website
https://nodejs.org/en/

after NPM is installed and MongoDB is up,make sure you are connected to the internet, and follow the next steps:
* clone the repo
* start MongoDB
* cd to the repo dictionary
* type 'npm install'
* create new file, call it .env, and add the phrase "SECRET={your own string}"
* type 'cd ./client'
* type 'npm install'
* type 'npm start'
* in a new terminal, cd to the repo
* type 'npm start'
* open https://localhost:4200

explaination:
by calling 'npm install', you are calling NPM to view the packages on package.json, which is the dependencies list of the project. and locally installing every dependency missing.
both the repo and the client dictionary are needed to be initialized on their own, since they are seperated entities

client contains a script, that is called 'npm start', that compile the html files and render Angular. it also initialize nodemon, which recompile the project whenever a change is made

the repo contains a script, which also called 'npm start', that initialize the MongoDB scheme and start basic HTML server which is connected to the frontend


hope you enjoyed my basic website, and sorry for all the problem I caused, thanks for the amazing 3 years Yuri <3
