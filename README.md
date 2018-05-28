## django-docker starter

<https://docs.docker.com/compose/django/#create-a-django-project>

- Create the Django project
```sh
sudo docker-compose run web django-admin.py startproject <project-name> .
```

- Connect db in `<project-name>/settings.py`
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'HOST': 'db',
        'PORT': 5432,
    }
}
```

- Start app on <http://localhost:8000>
```sh
docker-compose up
```
