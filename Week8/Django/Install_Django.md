### How To Create a New Django Project 

#### On *Windows*

1. Create a new project
2. Create a virtual environment
3. Activate the virtual environment
4.	Add requirements.txt with this command in your terminal `copy NUL requirements.txt`
    `Django==2.1.4`
5.	Install requirements with pip:
    `pip install -r requirements.txt`
6.	Create Django project:
    `django-admin startproject project_name (no hyphens)`
7.	Create an app next to the project directory:
    `python manage.py startapp app_name`
8.	You’re done!

##### Some more help
1. How to quickly open the current directory from the command prompt?
     `start .`

#### On *Mac*

1. Create a new project
2. Create a virtual environment
3. Activate the virtual environment
4.	Add requirements.txt with this command in your terminal `touch requirements.txt`
    `Django==2.1.4`
5.	Install requirements with pip:
    `pip install -r requirements.txt`
6.	Create Django project:
    `django-admin startproject project_name (no hyphens)`
7.	Create an app next to the project directory:
    `python manage.py startapp app_name`
8.	You’re done!

##### Some more help
1. How to quickly open the current directory from the command prompt?   
    `open .`

1. A command to see the hidden files in the terminal is :
    `ls -a`

2. A command to create a directory :
    `mkdir name_of_a_directory`

3. A command to get to the previous directory is :
    `cd ..`

#### Common errors
1. Unresolved reference: 'django' error in PyCharm

Solution: Peform following steps.
    1. In preference/settings go to Project > Project Interpreter
    2. On the right hand side click on settings icon >  Add Local
    3. Select correct Python version from Base Interpreter
    4. Mark the checkbox against Inherit global site-packages and Make available to all projects
    5. Click "ok" 
    6. Once this is done in Project Intepreter you will be able to see Django in the Package list.

2. Get out of the virtual environement :
    `deactivate`

3. Install a package in a virtual env : 
    `pip3 install package_name`

4. Install a specific version of a package :
    `pip3 install package_name==2.1.2`

5. Upgrade a package :
    `pip3 install –upgrade package_name`


