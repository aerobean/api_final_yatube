# API Yatube

API для социальной сети Yatube.

## Возможности

- Просмотр постов без необходимости авторизации
- Написание постов для авторизированных пользователей
- Группировка постов по группам и по авторам
- Создание, просмотр и удаление комментариев к постам
- Подписка и отписка на авторов

## Технологии

- [Python 3.7.0](https://www.python.org)
- [Django 3.2.14](https://www.djangoproject.com)
- [djangorestframework 3.12.4](https://www.django-rest-framework.org)


## Установка

Скопируйте репозиторий в свою папку:
```sh
$git clone https://github.com/aerobean/api_final_yatube.git
```

Установите виртуальное окружение:
```sh
$python3 -m venv <myenvname>
```

После установки запустите его:
```sh
$source <myenvname>/scripts/activate
```

Установите зависимости из requirements.txt:
```sh
$pip install -r reqiurements.txt
```

Выполните миграции:
```sh
$cd yatube_api
$python3 manage.py makemigrations
$python3 manage.py migrate
```

Запустите сервер:
```sh
$python3 manage.py runserver
```

API доступен по адресу http://127.0.0.1:8000/api/v1/

## Документация

Документация в ReDoc по ссылке: http://127.0.0.1:8000/redoc/#tag/api
