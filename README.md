# py_docker_template

Create your project:

    sudo docker-compose run web django-admin startproject <PROJECT_NAME> .

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

Run the server:

    docker-compose up
