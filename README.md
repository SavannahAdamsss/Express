# Express
Learning Express:

Beginnings:


//Create repo
//Cd into repo
//Npm init 
//Git init
//Npm install cors
//Copy and paste the code below (same every time)
//Npm install express
//Node index.js
     //(After node App is listening on 3000)
     //app.listen(3000 || process.env.PORT, () => console.log('Example app listening on port 3000!'));

const express = require('express');
const app = express();

app.get('/', (req, res) => res.send('Hello World!'));

app.listen(3000 || process.env.PORT, () => console.log('Example app listening on port 3000!'));



Simple form:

const express = require('express')
const app = express()

app.get('/', (req, res) => res.send('Hello World!'))

app.listen(3000, () => console.log('Example app listening on port 3000!'))

* This app starts a server and listens on port 3000 for connections. The app responds with “Hello World!” for requests to the root URL (/) or route. For every other path, it will respond with a 404 Not Found.  https://ic9atfvn9ama.runkit.sh/

* The example above is actually a working server: Go ahead and click on the URL shown. You’ll get a response, with real-time logs on the page, and any changes you make will be reflected in real time. This is powered by RunKit, which provides an interactive JavaScript playground connected to a complete Node environment that runs in your web browser. Below are instructions for running the same app on your local machine.

13:25:58.029 
"Example app listening on port 3000!"
13:25:58.029 
Request GET / ip=128.177.113.102id=3e56eb5dbc1a
13:25:58.039 
Response GET / status=200duration=1340id=3e56eb5dbc1a
13:25:58.256 
Request GET /favicon.ico ip=128.177.113.102id=df42c609877e
13:25:58.262 
Response GET /favicon.ico status=404duration=34id=df42c609877e


Running Locally:

* First create a directory named myapp, change to it and run npm init. Then install express as a dependency, as per the installation guide.

* In the myapp directory, create a file named app.js and copy in the code from the example above.

Run the app with the following command:

$ node app.js
Then, load http://localhost:3000/ in a browser to see the output.



Installing: 

* Assuming you’ve already installed Node.js, create a directory to hold your application, and make that your working directory.

* $ mkdir myapp
* $ cd myapp
* Use the npm init command to create a package.json file for your application. For more information on how package.json works, see Specifics of npm’s package.json handling.

* $ npm init
* This command prompts you for a number of things, such as the name and version of your application. For now, you can simply hit RETURN to accept the defaults for most of them, with the following exception:

* entry point: (index.js)
* Enter app.js, or whatever you want the name of the main file to be. If you want it to be index.js, hit RETURN to accept the suggested default file name.

* Now install Express in the myapp directory and save it in the dependencies list. For example:

* $ npm install express --save
* To install Express temporarily and not add it to the dependencies list:

* $ npm install express --no-save
