# edblog
Django Project

### Set up and activate a virtual environment in Windows/Bash using Python3

py -m venv env

source env/Scripts/activate

#### Set up and activate a virtual environment in Windows/Bash using Python2.7 (not recommend)

virtualenv env

source env/bin/activate

### Install Django and create a project folder

python -m django --version
(my version is 3.0.8)

django-admin startproject <django-pro>
(_startproject_ will create a folder containing __init__.py, settings.py, urls.py and wsgi.py for you)
