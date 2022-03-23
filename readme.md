# Django framework instructions and guidance

#==============================================================================
Create a main project folder using your command line terminal. Then open that project folder in vs code. Then enter the commmand, 'pipenv shell', to create a virtual environement for your django project.
#===============================================================================

Then copy and paste the following packages:

[packages]
django = "==3.0.8"
psycopg2-binary = "_"
coverage = "_"

[dev-packages]
isort = "==5.2.1"
flake8 = "==3.8.3"
black = "==19.10b0"
factory-boy = "==2.12.0"
django-nose = "==1.4.7"

into your Pipfile that was created when you created your virtual environment then enter the command 'pipenv install --dev' to install these packages into your virtual environement.

#============================================================================

Then create a setup.cfg file inside your main project folder. Then copy and paste the following content:

[flake8]
ignore = E203, E266, E501, W503
max-line-length = 88
max-complexity = 18
select = B,C,E,F,W,T4

[isort]
multi_line_output=3
include_trailing_comma=True
force_grid_wrap=0
use_parentheses=True
line_length=88

into your setup.cfg file.

#===============================================================================

Then enter the command, 'django-admin startproject project .', to create project folder for your app within the main prokect folder. Then craete a app folder by using the command, 'python manage.py startapp appname' or django-admin startapp appaname'. The appname can be named anything you want e.g.
python manage.py startapp todo. However, you should name your project folder for your app, project to avoid confusion between your app folder and project folder.

#===============================================================================

Then enter the command, 'python manage.py runserver', to start a django development server.
