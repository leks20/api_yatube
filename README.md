
# API_Yatube

REST API для социальной сети блогеров [Yatube](https://blog-yatube.tk) (созданы в рамках учебного курса Яндекс.Практикум).
Аутентификация по JWT-токену

## Стек технологий
- проект написан на Python с использованием Django REST Framework
- библиотека Simple JWT - работа с JWT-токеном
- развернут на сервере Яндекс.Облако - nginx, ginicorn
- система управления версиями - git

## Как запустить проект:

1) Клонируйте репозитроий с проектом:
```
git clone https://github.com/leks20/api_yatube
```
2) В созданной директории установите виртуальное окружение, активируйте его и установите необходимые зависимости:
```
python3 -m venv venv

. venv/bin/activate

pip install -r requirements.txt
```
3) Создайте в директории файл .env и поместите туда SECRET_KEY, необходимый для запуска проекта

4) Выполните миграции:
```
python manage.py migrate
```
5) Создайте суперпользователя:
```
python manage.py createsuperuser
```
6) Запустите сервер:
```
python manage.py runserver
```
____________________________________

Ваш проект запустился на http://127.0.0.1:8000/

Полная документация ([redoc.yaml](https://github.com/leks20/api_yatube/blob/master/static/redoc.yaml) доступна по адресу http://localhost:8000/redoc/ 

С помощью команды *pytest* вы можете запустить тесты и проверить работу модулей
