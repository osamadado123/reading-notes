# Custom User Model
for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.
## Setup
To start, create a new Django project from the command line. We need to do several things:

create and navigate into a dedicated directory called accounts for our code
install Django
make a new Django project called django_project
make a new app accounts
start the local web server
Here are the commands to run:

## Windows

- cd onedrive\desktop\code
- mkdir pages
- cd pages
- python -m venv .venv
- .venv\Scripts\Activate.ps1
- (.venv) > python -m pip install django~=4.0.0
- (.venv) > django-admin startproject django_project .
- (.venv) > python manage.py startapp accounts
- (.venv) > python manage.py runserver

## macOS

- % cd ~/desktop/code
- % mkdir pages
- % cd pages
- % python3 -m venv .venv
- % source .venv/bin/activate
- (.venv) % python3 -m pip install django~=4.0.0
- (.venv) % django-admin startproject django_project .
- (.venv) % python3 manage.py startapp accounts
- (.vent) % python3 manage.py runserver

### In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call our custom user model CustomUser. Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.

![my img](https://scontent.xx.fbcdn.net/v/t1.15752-9/318030386_2972381146400726_7809578650831175440_n.png?_nc_cat=103&ccb=1-7&_nc_sid=aee45a&_nc_eui2=AeGEf74dMj7xYmisocEXFY6GwM1IhtYaVWvAzUiG1hpVa-k2dM1SRUV5UOC_5dnTu31jN3uUg4rzyOo8ghkDSd4F&_nc_ohc=NY0bT7qLx00AX8bX_Mz&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AdRL-RjZPaK8ldyJKqzBQGOXaV17RrP44g3dRVf_T8-DSA&oe=63B59E19)