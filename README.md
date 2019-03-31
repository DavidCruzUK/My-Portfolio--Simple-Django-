# Simple Porfolio web (Django2)

## Getting Started
This Project is created with python3 with Django2:
Please find here the dependencies:
```
Django==2.1.7
Pillow==5.4.1
psycopg2==2.7.7
psycopg2-binary==2.7.7
pytz==2018.9
```
You also will need PostgreSQL, I personally use the following app on my Mac
http://postgresapp.com/

### Installing
1st Create a virtual server:
```
$ python3 -m venv {{path_to_venv}}/{{project_name}}
```
2nd Activate the created virtual server:
```
$ source {{path_to_venv}}/{{project_name}}/bin/activate
```
3rd After initialise your PostgresSQL Database:

Modify the file settings.py inside of portfolio-project/porfolio folder with your settings.
Note: By default the port number is 5432
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'portfoliodb',
        'USER': 'postgres',
        'PASSWORD': '1234',
        'HOST': 'localhost',
        'PORT': '5431',
    }
}
```
4rd create a superuser
```
$ django-admin createsuperuser
```

5th you must be ready to go
