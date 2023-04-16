# Используемые команды:

### установка джанго версии 2.1.5 (на версии 2 ошибка с таблицей)

	pipenv install django==2.1.5

### запуск виртуальной среды в директории

	pipenv shell

### создание проекта

	django-admin startproject mb_project .

### создание приложения внетри проекта

	python manage.py startapp posts

### создание исходной базы данных по умолчанию

	python manage.py migrate

## создания суперпользователя

	python manage.py  createsuperuser

### запуск сервера на localhost:8000

	python manage.py runserver

### создание файла миграции, который является ссылкой на все новые изменения в наших моделях

	python manage.py makemigrations post

###  создание фактической базы данных, которая выполняет инструкции в файле migrations

	python manage.py migrate posts

### остановка локального сервера Ctrl+c и выход из виртуальной среды

	exit

### запуск тестирования

	python manage.py test

### установка heroku

	curl https://cli-assets.heroku.com/install-ubuntu.sh | sh

### установка веб сервера в виртуальную среду

	pipenv install gunicorn
