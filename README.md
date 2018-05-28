## django-docker starter

<https://docs.docker.com/compose/django/#create-a-django-project>

Create the Django project by running the docker-compose run command as follows:
```sh
sudo docker-compose run web django-admin.py startproject composeexample .
```
This instructs Compose to run `django-admin.py startproject composeexample` in a container, using the `web` service’s image and configuration.
