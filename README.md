# Проект «API для Yatube»

## Описание проекта:
### *Сервис позволяет пользователям отправлять запросы к Базе Данных для получения групп, постов, комментов и подписок . Авторизованным пользователям доступны функции создания/редактирования/удаления постов и комментариев из Базы Данных .*

 ## Как запустить проект:
 - #### Клонировать репозиторий и перейти в него в командной строке: ` git@github.com:Efesov/api_final_yatube.git`
- #### Cоздать и активировать виртуальное окружение: `python -m venv env` / `source venv/Scripts/activate`
- #### Установить зависимости из файла requirements.txt: `python -m pip install --upgrade pip` / `pip install -r requirements.txt`
- #### Выполнить миграции: `python manage.py makemigrations` / `python manage.py migrate`
-  #### Запустить проект: `python manage.py runserver`
 ---
 ### Примеры запросов:
 - `/api/v1/posts/ (GET, POST, PUT, PATCH, DELETE)`

- `/api/v1/posts/{post_id}/comments/ (GET, POST, PUT, PATCH, DELETE)`

- `/api/v1/groups/ (GET)`

- `/api/v1/follow/ (GET, POST)`

## *Использованные технологии:*
<div>
<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/python/python-original.svg" title="Python" alt="Python" width="90" height="90"/>&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/django/django-plain-wordmark.svg" title="django"  alt="django" width="90" height="90"/>&nbsp;
</dev>

