# edblog
Django Project

### Set up and activate a virtual environment in Windows/Bash using Python3
mkdir < django-project > 

cd django-project

py -m venv env

source env/Scripts/activate

#### Set up and activate a virtual environment in Windows/Bash using Python2.7 (not recommend)

virtualenv env

source env/bin/activate

### Install Django and create a project folder

python -m django --version
(my version is 3.0.8)

django-admin startproject < edblog >

Note: _startproject_ will create a folder containing __init__.py, settings.py, urls.py and wsgi.py for you.

### Create the app for the project and run the server at port 8000
python manage.py startapp < blog >

cd edblog

python manage.py runserver

Note: Open the browser and go to localhost:8000/admin, you'll see the admin login page running successfully.
