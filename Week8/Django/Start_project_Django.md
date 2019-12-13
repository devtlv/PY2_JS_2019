### Starting with Django

#### Making sure Pip installed
    `python3 -m pip install --user --upgrade pip`

####  Installing virtualenv
    `python3 -m pip install --user virtualenv`

####  Creating a virtualenv
    `python3 -m virtualenv env`
The second argument is the location to create the virtualenv. Generally, you can just create this in your project and call it env.
`virtualenv` will create a virtual Python installation in the env folder.

####  Activating a virtualenv
    `source env/bin/activate`

#### Using requirements files
Instead of installing packages individually, pip allows you to declare all dependencies in a Requirements File. For example you could create a requirements.txt file containing:
    `Django==2.1.3`
And tell pip to install all of the packages in this file using the -r flag:
    `pip3 install -r requirements.txt`

#### Freezing dependencies
Pip can export a list of all installed packages and their versions using the freeze command:
    `pip3 freeze`

####  Installing Django
    `pip3 install -r requirements.txt`
This will install Django and django-admin a tool that lets you start Django projects.

####  Start a Django project
    `django-admin startproject first_project`

#### Launching Django
    ```
    cd first_project
    python3 manage.py runserver
    ```
#### Creating a Django app
Make sure your virtual env is activated!
    `python3 manage.py startapp first_app`

#### Declaring your app at the project level
> first_project/settings.py
```
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    # adding our first app
    'first_app',
]
```
#### Run the server to make sure it works:
    `python3 manage.py runserver`