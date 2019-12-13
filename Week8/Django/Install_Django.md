### How To Create a New Django Project 

#### On *Windows*

1. Create a new project
2. Create a virtual environment
3. Activate the virtual environment
4.	Add requirements.txt with this command iyour terminal `copy NUL requirements.txt`
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
    Write this command in your terminal `start .`

#### On *Mac*

1. Create a new project
2. Create a virtual environment
3. Activate the virtual environment
4.	Add requirements.txt with this command iyour terminal `touch requirements.txt`
    `Django==2.1.4`
5.	Install requirements with pip:
    `pip install -r requirements.txt`
6.	Create Django project:
    `django-admin startproject project_name (no hyphens)`
7.	Create an app next to the project directory:
    `python manage.py startapp app_name`
8.	You’re done!

##### Some more help


#### Common errors
1. Unresolved reference: 'django' error in PyCharm

Solution: Peform following steps.
1. In preference/settings go to Project > Project Interpreter
2. On the right hand side click on settings icon >  Add Local
3. Select correct Python version from Base Interpreter
4. Mark the checkbox against Inherit global site-packages and Make available to all projects
5. Click "ok" 

Once this is done in Project Intepreter you will be able to see Django in the Package list.



