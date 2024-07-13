docker-compose run --rm app sh -c "django-admin startproject app ."
docker-compose run --rm app sh -c 'python manage.py startapp helpers'
docker compose run --rm app sh -c 'python manage.py wait_for_db'
