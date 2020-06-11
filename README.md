# py_docker_template

Create your project:

    docker-compose run web django-admin startproject <PROJECT_NAME> .

Update your database settings in <PROJECT_NAME>/settings.py

    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'postgres',
            'USER': 'postgres',
            'PASSWORD': 'postgres',
            'HOST': 'db',
            'PORT': 5432,
        }
    }

Run initial migrations

    docker-compose run web ./manage.py migrate

Create a superuser

    docker-compose run web ./manage.py createsuperuser

Run the server:

    docker-compose up

Verify the server is up:

    visit http://localhost:8000/admin
