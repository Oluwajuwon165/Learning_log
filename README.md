# Project Name: Learning Log
## Introduction
This is a web application that allows users to keep track of topics they are learning about and make entries on each topic. The application was built as a final project for the ALX SE foundations days. The resource used was Python Crash Course book by Eric Matthes.

## Link to the deployed site:
I'm currently having some difficulties deploying the app. This part of the README will be updated as soon as I get to deploy the app.

## Final project blog article: https://medium.com/@ollyjhay
The path to the article will be update in the link, later today.

## Author: Oladiti Oluwajuwon

## Author's LinkedIn: https://www.linkedin.com/in/oladiti-oluwajuwon

## Installation
### To run the application locally, you will need to:

**Clone the project repository and navigate to the root directory of the project. To clone the repo, run this command:**
```
$ git clone https://github.com/Oluwajuwon165/Learning_log.git
```

**Create a virtual environment for the project using the following command:**
```
learning_log$ python -m venv ll_env
```
**Note that the name of the new directory, ll_env, is arbitrary and can be changed. Also, you are not meant to include "learning_log$" while running the command**

**In this instance, we're executing the venv module to generate a virtual environment named ll_env. A possible erro you may get is this:**
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
**You don't have to deactivate the virtual environment. It is needed to run this application. That was just to show you how to deactivate it when you are done.**
**In the active virtual environment, upgrade pip and install Django using the following commands:**
```
(ll_env)learning_log$ pip install --upgrade pip
```
```
(ll_env)learning_log$ pip install django
```
The output of successful commands for the Django installation should be similar to the following:
```
Collecting django
  Downloading Django-4.2-py3-none-any.whl (8.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.0/8.0 MB 166.9 kB/s eta 0:00:00
Collecting backports.zoneinfo
  Using cached backports.zoneinfo-0.2.1-cp38-cp38-manylinux1_x86_64.whl (74 kB)
Collecting sqlparse>=0.3.1
  Using cached sqlparse-0.4.3-py3-none-any.whl (42 kB)
Collecting asgiref<4,>=3.6.0
  Using cached asgiref-3.6.0-py3-none-any.whl (23 kB)
Installing collected packages: sqlparse, backports.zoneinfo, asgiref, django
Successfully installed asgiref-3.6.0 backports.zoneinfo-0.2.1 django-4.2 sqlparse-0.4.3
```
**Install the modules django-bootstrap5 and platformshconfig, which are listed in the requirements.txt file, using the following commands:**
```
(ll_env)learning_log$ pip install django-bootstrap5
```
```
(ll_env)learning_log$ pip install platformshconfig
```
**Apply the migrations for the apps by running the following command:**
```
(ll_env)learning_log$ python manage.py migrate
```
**You should see an output like this:**
```
Operations to perform:
  Apply all migrations: admin, auth, contenttypes, learning_logs, sessions
Running migrations:
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  Applying admin.0001_initial... OK
  Applying admin.0002_logentry_remove_auto_add... OK
  Applying admin.0003_logentry_add_action_flag_choices... OK
  Applying contenttypes.0002_remove_content_type_name... OK
  Applying auth.0002_alter_permission_name_max_length... OK
  Applying auth.0003_alter_user_email_max_length... OK
  Applying auth.0004_alter_user_username_opts... OK
  Applying auth.0005_alter_user_last_login_null... OK
  Applying auth.0006_require_contenttypes_0002... OK
  Applying auth.0007_alter_validators_add_error_messages... OK
  Applying auth.0008_alter_user_username_max_length... OK
  Applying auth.0009_alter_user_last_name_max_length... OK
  Applying auth.0010_alter_group_name_max_length... OK
  Applying auth.0011_update_proxy_permissions... OK
  Applying auth.0012_alter_user_first_name_max_length... OK
  Applying learning_logs.0001_initial... OK
  Applying learning_logs.0002_entry... OK
  Applying learning_logs.0003_topic_owner... OK
  Applying sessions.0001_initial... OK
```
That's all, for the configurations.

**Start the development server by running the following command:**
```
(ll_env)learning_log$ python manage.py runserver
```
**Note that you need to run this command from the root of the project directory.**\n
A successful output should look like this:
```
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
April 05, 2023 - 11:22:52
Django version 4.2, using settings 'll_project.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

The output shows your server is running on http://127.0.0.1:8000/\n
You can specify a different port other than 8000 if you intend not to use the default port of the Django's development server using the command:
```
(ll_env)learning_log$ python manage.py runserver 8080
```
The specified command above designates port 8080, however, any port that is currently available can be selected for use.

## Usage
**Once the application is running, navigate to http://127.0.0.1:8000/ (if you used the default port) in your web browser to access the homepage. From there, you can create a new account, log in, and start keeping track of your learning topics and entries.**

## Contributing
Contributions to this project are welcome. If you would like to contribute, please fork this repository and submit a pull request.


## Story
As a lifelong learner, I often find myself struggling to remember all the topics I've studied over time. That's why I was excited to work on the Learning Log project as part of the Python Crash Course book.

The technical challenge I set out to solve was to create a web application that is easy to use and allows users to keep track of their learning progress over time. I decided to use Django as the web framework and SQLite as the database.

One of the main challenges I faced was was the deployment of the app. I encountered different challenges while I tried to deploy. As of the time of crafting this README, I'm yet to deploy the app. I'm already considering other platforms for my deployment. I hope to get that fixed as soon as possible.

Overall, I am very happy with the outcome of the project and I have already started using it to keep track of my own learning progress. In the future, I would like to add more features such as search functionality to make it even more useful.

**Thanks to Eric Matthes, for the inspiration behind this project.**

