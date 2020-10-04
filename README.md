# reverse-engineering

# ABOUT
This authentication app allows users to create an account, log into the account and sign back out securely. 
All user data is stored in a mysql database.

# USER STORY
As a user signs-up.

The users info will be stored in a mysql database.

A user can then log in.


# TECHNOLOGIES USED

-EXPRESS 

-MYSQL

-SEQUELIZE

-NodeJS


# GETTING STARTED TUTORIAL
To begin using this app clone this repository into your local storage. Once this is complete, do the following steps:

1) Create a mysql db called "passport_demo" 
2) Go into the config file, open config.js and insert your personal data; username and password.
3) Open a terminal in the current repo and run "npm i" to install all node packages.
4) In the terminal run "node server.js" to successfully connect to server,
5) Open the browser and type "http://localhost:8080" in search bar.
6) You now can sign-up and log in.

# FILES PURPOSE
CONFIG

MIDDLEWARE

Authenticated.js - restricts the routes that a user is not allowed to visit if not logged in. If the user is logged in, it will continue

config.json - connection is the configuration to connect to server

passport.js - contains javascript logic that tells passport we want to log in with an email address and password

MODELS

index.js - connects to database and imports users log in data

user.js - requires "bcrypt" for password hashing. This makes our database secure even if compromised. Here we have a JS that defines what is stored on our database

ROUTES

api-routes.js - contains routes for signing in, logging out and getting users specific data to be displayed on the client side

html-routes.js - routes that check whether user is signed in, whether the user already has an account and sends them to the correct html page 

package.json - contains all package info, node modules used, version info, etc

server.js - requires packages, sets up the PORT, creates express and middleware, creates routes and syncs database and logs a message in the terminal on successful connection to server 
