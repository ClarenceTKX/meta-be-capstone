# meta-be-capstone
Welcome to my capstone project for the Meta Back-end Developer Course. To start, please run the following commands:
```
git clone https://github.com/ClarenceTKX/meta-be-capstone
cd meta-be-capstone
python -m pipenv install
pip install mysqlclient django-admin djangorestframework djoser django-filter markdown
cd littlelemon
python manage.py runserver
```
For the database portion, please run the following commands in your respective workbenches/using the connector.cursor class: 
```
CREATE DATABASE littlelemon;
USE littlelemon;
CREATE USER 'django@localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON littlelemon.* TO 'django@localhost';
```

# Testing
To execute unittests provided under the `tests` directory, run the following commands. 
Please ensure that `pipenv` is activated and you are in the `littlelemon` main directory.
```
python manage.py test ./tests
```
For the purposes of this project, the auxiliary authentication details are as follows:
```
user: django
password: password
```