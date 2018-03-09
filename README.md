# Insta Fight
## Description
This is a web application to compare two accounts on instagram in this way: You give the two accounts and the app will take the last uploads from both and respond with the account with the most likes.

## Motivation
This is a project for a [web development class](http://johnguerra.co/classes/webDevelopment_spring_2018/) in [Uniandes](https://www.uniandes.edu.co). The objective is to make a quick project using node, MongoDB and ReactJS.

## Getting Started
For this proyect to run you will need a couple of things first. First of all, a package manager. I recommend [npm](https://www.npmjs.com/) for this project.

Once you have a package manager you can now download this repo on any folder you want on your computer.

The next thing you have to do before you can deploy is setting up a mongo database. To do this:
* You can download mongodb [here](https://www.mongodb.com), then make a new database and a collection with the name you want.
* Or you can also use [mongolab](mlab.com) for free. 

What you need to do now is set up ENV variables for the project before you can deplyo. This is important because this is how the project will connect to the db and how you can also set up your preferred port for the back-end server of this program. To do this step you can:
* Manually configuring environmental variables in your OS using the terminal or any other way your OS allow you to do that.
* Add a file called `.env` and set the variables there.

The veriables you need to add are:
* `PORT` : This is the port you want the server to run on.
* `URL` : The url where mongo is listening, this can be something like `mongodb://localhost:xxxx/<dbname>` or `mongodb://<user>:<pass>@dsxxxxx.mlab.com:xxxx/<dbname>` if you are using mongo lab.
* `DBNAME` : The name of the database you want to connect to.
* `COLLECT` : The name of the collection inside the database you want to use for this project. Try to have this collection empty before deploying as well.

## Deployment
Once you have everything ready open the terminal on the root folder where this project is downloaded in your pc and then enter on the `frontend` folder and run:
* ```npm install```
* ```npm start build```

that way you will have the Reactjs front end application ready. Now, open a new terminal, go back to the main folder and run:
* ```npm install```
* ```npm start```

Then the node-express server will be up and running. Once you are finish with this you can open `localhost:3000` on your favorite browser and you will se the homepage of the app.


## Authors
* [__Juan Sebastian Prieto__](https://jsprieto10.github.io)

## Contributing
If anyone wants to give me any help or ideas, you can by making new [Issues](https://github.com/cawolfkreo/exam-web-dev/issues) or a [Pull requests](https://github.com/cawolfkreo/exam-web-dev/issues).

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository has the standard MIT license. You can find it [here.](https://github.com/cawolfkreo/exam-web-dev/blob/master/LICENSE)
