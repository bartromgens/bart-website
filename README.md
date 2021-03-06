bart-website
------------
[![Build Status](https://travis-ci.org/bartromgens/bart-website.svg?branch=master)](https://travis-ci.org/bartromgens/bart-website)

A personalizable personal website. 
Based on Django and Mezzanine. 
 
### Installation

##### Create a virtualenv and install dependencies
```
$ cd scripts
$ bash create_env.sh
```

##### Activate the virtualenv
```
$ source env/bin/activate
```

##### Create local settings
``` 
$ python scripts/create_local_settings.py 
```

##### Create database
``` 
$ python manage.py migrate 
```

##### Create superuser
``` 
$ python manage.py createsuperuser
```

##### Run a debug test server
``` 
$ python manage.py runserver
```

Login at http://127.0.0.1:8000/admin/ to create a homepage with '/' as URL.


#### Webfaction

Create a new Django 1.8.x + Python 3.x application in the webfaction web interface.


##### Install a user pip
```
$ easy_install-3.4 pip
```

##### Install dependencies
```
$ pip3.4 install --user -r requirements.txt 
```

##### Collect staticfiles
```
$ python3.4 manage.py collectstatic
```

##### Check error log
```
$ less ~/logs/user/error_bart_website.log
```

##### Apache restart
```
$ ~/webapps/bart_website/apache2/bin/restart
```
