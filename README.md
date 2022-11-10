# API Yatube

API для социальной сети Yatube.

## Автор

Будущий бэкендер [Максим Асташев](https://github.com/aerobean)

## Возможности

- Просмотр постов без необходимости авторизации
- Написание постов для авторизированных пользователей
- Группировка постов по группам и по авторам
- Создание, просмотр и удаление комментариев к постам
- Подписка и отписка на авторов

## Технологии

- [Python 3.9.10](https://www.python.org)
- [Django 2.2.15](https://www.djangoproject.com)
- [djangorestframework 3.12.4](https://www.django-rest-framework.org)


## Установка

Скопируйте репозиторий в свою папку:
```sh
git clone https://github.com/aerobean/api_final_yatube.git
```

Установите виртуальное окружение:
```sh
python3 -m venv venv
```

После установки запустите его:
```sh
source venv/bin/activate
```

Установите зависимости из requirements.txt:
```sh
pip install -r requirements.txt
```

Выполните миграции:
```sh
cd yatube_api
python3 manage.py makemigrations
python3 manage.py migrate
```

Запустите сервер:
```sh
python3 manage.py runserver
```

API доступен по адресу http://127.0.0.1:8000/api/v1/

## Документация

Документация в ReDoc по ссылке: http://127.0.0.1:8000/redoc/#tag/api

### Примеры запросов к API:

Получить список всех постов (GET):
```
http://127.0.0.1:8000/api/v1/posts/
```

Получить определенный пост (GET):
```
http://127.0.0.1:8000/api/v1/posts/1/
```

Получить коментарии определенного поста (GET):
```
http://127.0.0.1:8000/api/v1/posts/1/comments/
```

Получить список всех групп (GET):
```
http://127.0.0.1:8000/api/v1/groups/
```

Создать новый пост (POST):

(Требуется аутентификация)
```
http://127.0.0.1:8000/api/v1/posts/
```
