venv:
	source ../venv/bin/activate
	
run:
	python manage.py runserver

mi:
	python manage.py migrate

mig:
	python manage.py makemigrations 

shell:
	python manage.py shell

cuser:
	python manage.py createsuperuser

test:
	python manage.py test

cs:
	python manage.py collectstatic

flush:
	python manage.py flush

smig:
	python manage.py showmigrations

check:
	python manage.py check

i:
	pip install -r requirements.txt

freeze:
	pip freeze > requirements.txt

clean:
	find . -name "*.pyc" -delete
	find . -name "__pycache__" -type d -exec rm -rf {} +

help:
	@echo "Available commands:"
	@echo "  run              - Start Django development server"
	@echo "  migrate          - Apply database migrations"
	@echo "  makemigrations   - Create new migrations"
	@echo "  shell            - Open Django shell"
	@echo "  createsuperuser  - Create Django admin user"
	@echo "  test             - Run tests"
	@echo "  check            - Check for issues"
	@echo "  clean            - Clean Python cache files"
	@echo "  install          - Install requirements"
	@echo "  freeze           - Update requirements.txt"

dev-setup:
	python manage.py makemigrations
	python manage.py migrate
	python manage.py runserver

.PHONY: run migrate makemigrations shell createsuperuser test collectstatic flush showmigrations check install freeze clean help dev-setup
