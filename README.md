# Django: The powerful and flexible toolkit for building Web APIs.


![Django intro](django_boiler_plate/static/images/django-logo.png)

Author : Lija G

This is a boilerplate for Django Rest Framework designed and adopted by the Python developers at Accubits Technologies Inc. A basic user enrollment and verification application is implemented in this to provide a walk through the project structure.

This boilerplate enables the team to quickly setup a Django project environment with the adopted guidelines and helps new joiners to quickly get on board with us.

<br>

### Run app in local machine with dev , staging or production configurations
It's easier to debug issues in staging environment, if we can connect to staging db and other services from our local machine.
  
**Steps**
- Duplicate .env file with name `.env.staging` and update all staging config
- Run app using  
Linux - `export ENVIRON=staging && python manage.py runserver`
Windows - `set ENVIRON=staging && python manage.py runserver`

### Database Configuration
** MYSQL **
DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.mysql',
         'NAME': "db_name",
         'USER': 'user',
         'PASSWORD': 'password',
         'HOST': 'host',
         'PORT': 'port'
     }
 }

** POSTGRESS **
DATABASES = {
	'default': {
		'ENGINE': 'django.db.backends.postgresql_psycopg2',
		'NAME': 'db_name',
		'USER': 'user',
		'PASSWORD': 'password',
		'HOST': 'host',
		'PORT': 'port',
	}
}

** SQLITE **
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}
 