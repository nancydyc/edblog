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

### Install Django and create an edblog project folder

python -m django --version
(my version is 3.0.8)

django-admin startproject < edblog >

Note: _startproject_ will create a folder containing __init__.py, settings.py, urls.py and wsgi.py for you.

### Create the blog app and run the server at port 8000
python manage.py startapp < blog >

cd edblog

python manage.py runserver

Note: Open the browser and go to localhost:8000/admin, you'll see the admin login page running successfully.

### Create a superuser for admin login
In edblog directory, run the following commands:

python manage.py makemigrations

python manage.py migrate

python manage.py createsuperuser

(If it doesn't prompt you to create username and password, run-- 

   _winpty python manage.py createsuperuser_)
   
 You'll be able to enter a username, email address and password (twice) for the super user.
 
 Note: Now, navigate to local host:8000/admin, you can login with the username and password you just created and have a tour for Django site administration. 
