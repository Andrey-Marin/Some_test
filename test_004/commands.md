# Используемые команды:

### установка виртуальной среды

	pip3 install pipenv

### установка джанго версии 2

	pipenv install django==2.0

### запуск виртуальной среды в директории

	pipenv shell

### создание проекта

	django-admin startproject new_project .

### создание приложения внетри проекта

	python manage.py startapp pages

### запуск сервера на localhost:8000

	python manage.py runserver

### остановка локального сервера Ctrl+c и выход из виртуальной среды

	exit

### запуск тестирования

	python manage.py test
