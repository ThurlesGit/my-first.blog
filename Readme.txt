Create virtual environment (also called a virtualenv). Virtualenv will isolate your Python/Django setup on a per-project basis.

    c:\djangogirls>c:\Python34\python -m venv myvenv

Start your virtual environment by running:

    command-line
    C:\Users\Name\djangogirls> myvenv\Scripts\activate

Install Django

(myvenv) ~$ pip install django~=1.10.0
        Collecting django~=1.10.0
        Downloading Django-1.10.4-py2.py3-none-any.whl (6.8MB)
        Installing collected packages: django
        Successfully installed django-1.10.4

The first step is to start a new Django project. Basically, this means that we'll run some scripts provided by Django that will create the skeleton of a Django project for us. This is just a bunch of directories and files that we will use later.

    (myvenv) c:\djangogirls>django-admin.py startproject mysite .


NOTE update setting according to  https://tutorial.djangogirls.org/en/django_start_project/

Start server
    (myvenv) c:\djangogirls>python manage.py runserver

Creating an application

To keep everything tidy, we will create a separate application inside our project. It is very nice to have everything organized from the very beginning. To create an application we need to run the following command in the console (from djangogirls directory where manage.py file is):
    (myvenv) c:\djangogirls>python manage.py startapp blog


Creat a super user
    command-line
    C:\Users\Name\djangogirls>python manage.py createsuperuser



    python manage.py migrate blog
