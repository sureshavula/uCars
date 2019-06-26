# uCars
Project is about designing a web application similar to carDekho/carTrade to help the users to search for the car they required.

# uCars
# Introduction

Search awesome new cars.

Answer some question and we will tell you the best car for you..!!!

# Developer Guide

## Live Website [Here](https://ucars-project.herokuapp.com/)

## How to run on local machine

### Method 1:
```bash

'''
clone this repo
'''

git clone https://github.com/sureshavula/uCars.git
cd uCars

'''
run autostart.sh from terminal
'''
chmod +x autostart.sh

./autostart.sh

'''
activate virtual environment
'''
source ../venv/bin/activate

'''
create superuser to access admin page
'''

python manage.py createsuperuser

'''
run the server 
'''

python manage.py runserver [port no.]

'''
goto to localhost:[port no.] by default port no. will 8000 
'''

```

### Method 2:
```bash
'''
First thing first clone this repo.
'''

git clone https://github.com/sureshavula/uCars.git

'''
create a virtual environment on parent directory
'''
cd ../
virtualenv -p python3 venv

'''
start the virtual environment and return to poject directory
'''
source venv/bin/activate
cd uCars/

'''
Install dependencies:
'''

pip install -r requirements/local.txt

'''
run migrations 
'''

python manage.py migrate

'''
run test.py to test database it should display OK
'''

python manage.py test

'''
load data from json file run command load_json [filename]
'''
python manage.py load_json dump.json

'''
create superuser to access admin page
'''

python manage.py createsuper

'''
run the server 
'''

python manage.py runserver [port no.]

'''
goto to localhost:[port no.] by default port no. will 8000 
'''
```





