# Develop

> package.json

- holds app information and dependencies

  > package-lock.json

  > server.js

- initializes application connection to the server
  -initializes middlewhere necessary to send POST data
- initializes tracking for login data
- requires routes
- syncs with database

## config

> passport.js

- initializes passport
- sets up passport criteria and logic
- exports passport

### middleware

> isAuthenticated.js

- restricted routes and not letting a user access restricted routes if they are not logged in

## models

> index.js
> business logic

- init sequelize connection
- use file system to obtain MySql data
  > user.js
- use sequelize to make user model and input data
  -compares password hash
- auto hash password so actual pass not stored in database

## node_modules

- where our node package modules live

## public

Public folder

### js

> login.js
> grabs html elements
> submit logic for the login form
> post route for login data

> members.js

- get request ot figure out which user is logged in
  > signjup.js
- form and input elements
  -signup form on click logic
- posts to the signup route

### stylesheets

-styling

> login.html
> -main page and login form
> members.html
> -redirect for logged in members
> signup.html
> -sign up form

### routes

> api routes.js
> html routes.js
