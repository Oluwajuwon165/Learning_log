# Project Name: Learning Log
## Introduction
This is a web application that allows users to keep track of topics they are learning about and make entries on each topic. The application was built as a final project for the Python Crash Course book by Eric Matthes.

## Link to the deployed site:
I'm currently having some difficulties deploying the app. This part of the README will be updated as soon as I get to deploy the app.

## Final project blog article: https://medium.com/@ollyjhay
The path to the article will be update in the link, later today.

## Author: Oladiti Oluwajuwon

## Author's LinkedIn: https://www.linkedin.com/in/oladiti-oluwajuwon

## Installation
### To run the application locally, you will need to:

**Clone the project repository and navigate to the root directory**.\n
**Create a virtual environment for the project using the following command:**
```
learning_log$ python -m venv ll_env
```
**Note that the name of the new directory, ll_env, is arbitrary and can be changed. Also, you are not meant to include "learning_log$" while running the command**
**In this instance, we're executing the venv module to generate a virtual environment named ll_env. A possible erro you may get is this:
```
Command 'python' not found, did you mean:

command 'python3' from deb python3
command 'python' from deb python-is-python3
```
To solve that, consider using the version of python that runs on your machine. Replace python with python3 in the command above. You should have something like this:
```
learning_log$ python3 -m venv ll_env
```
**Activate the virtual environment using the following command:**
```
learning_log$ source ll_env/bin/activate
```
When the environment is active, you’ll see the name of the environment in parentheses. Something like this:
```
(ll_env)learning_log$
```

This implies that it's possible to both install new packages to the environment and utilize packages that have already been installed. Any packages that are installed in ll_env will not be accessible when the environment is inactive.
To stop using a virtual environment, enter deactivate:
```
(ll_env)learning_log$ deactivate
```
You don't have to deactivate the virtual environment. It is needed to run this application. That was just to show you how to deactivate it when you are done.
**In the active virtual environment, upgrade pip and install Django using the following commands:
```
(ll_env)learning_log$ pip install --upgrade pip
(ll_env)learning_log$ pip install django
```
## Usage
**Once the application is running, navigate to http://localhost:8000 in your web browser to access the homepage. From there, you can create a new account, log in, and start keeping track of your learning topics and entries.**

## Contributing
Contributions to this project are welcome. If you would like to contribute, please fork this repository and submit a pull request.


## Story
As a lifelong learner, I often find myself struggling to remember all the topics I've studied over time. That's why I was excited to work on the Learning Log project as part of the Python Crash Course book.

The technical challenge I set out to solve was to create a web application that is easy to use and allows users to keep track of their learning progress over time. I decided to use Django as the web framework and SQLite as the database.

One of the main challenges I faced was implementing user authentication and authorization, which involved learning about session management and password hashing. I also had to figure out how to structure the database tables to store topics and entries in a scalable way.

Till now, though, I'm still having some challenge with deployment. I hope to get that fixed as soon as possible.

Overall, I am very happy with the outcome of the project and I have already started using it to keep track of my own learning progress. In the future, I would like to add more features such as tags and search functionality to make it even more useful.

**Thanks to Eric Matthes, for the inspiration behind this project.**
