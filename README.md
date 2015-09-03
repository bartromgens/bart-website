## bart-website

A personalizable website to personalize. 
Based on Django and Mezzanine. 
 
## Installation

Create a virtualenv with dependencies with the create_env.sh script.

Activate the virtualenv,

```
$ source env/bin/activate
```

Create local settings,

``` 
$ python scripts/create_local_settings.py 
```

Create database,

``` 
$ python manage.py migrate 
```

Create superuser,

``` 
$ python manage.py createsuperuser
```

Run a debug test server,

``` 
$ python manage.py runserver
```

Login at http://127.0.0.1:8000/admin/ to create a homepage with '/' as URL.


### Webfaction

Create a new Django 1.8.x + Python 3.4 application in the webfaction web interface.



