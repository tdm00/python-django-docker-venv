# Getting started

```
python3 -m venv .venv
pip install -r requirements.txt
django-admin startproject cfehome .
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
echo "DEBUG=1" > .env
gunicorn cfehome.wsgi:application --bind 0.0.0.0:8000
touch Dockerfile
```
