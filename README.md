# Проект «API для Yatube»

## Описание проекта:
### REST API для социальной сети Yatube .

- #### *Позволяет делать запросы к моделям проекта: Посты, Группы, Комментарии, Подписки .*
- #### *Поддерживает методы GET, POST, PUT, PATCH, DELETE* .
- #### *Предоставляет данные в формате JSON*
-  #### *Документация доступна по URL-адресу:  [http://127.0.0.1:8000/redoc/](http://127.0.0.1:8000/redoc/)*

 ## Как запустить проект:
 - #### Клонировать репозиторий и перейти в него в командной строке: ` git@github.com:Efesov/api_final_yatube.git`
- #### Cоздать и активировать виртуальное окружение: 
-  - ##### На Mac & Linux: `python3 -m venv env`/ `source env/bin/activate`
-  - ##### На Windows: `python -m venv venv` / `source venv/Scripts/activate`

- #### Установить зависимости из файла requirements.txt:
-  - ##### На Mac & Linux: `python3 -m pip install --upgrade pip` / `pip install -r requirements.txt`
-  - ##### На Windows: `python -m pip install --upgrade pip` / `pip install -r requirements.txt`
- #### Выполнить миграции: 
-  - ##### На Mac & Linux: `python3 manage.py migrate`
- - ##### На Windows: `python manage.py makemigrations` / `python manage.py migrate`
-  #### Запустить проект: 
-  - ##### На Mac & Linux: `python3 manage.py runserver`
-  - ##### На Windows: `python manage.py runserver`
 ---
 ### Примеры запросов:
 - `/api/v1/posts/ (GET, POST, PUT, PATCH, DELETE)`
 -  - `{
  "count": 123,
  "next": "http://api.example.org/accounts/?offset=400&limit=100",
  "previous": "http://api.example.org/accounts/?offset=200&limit=100",
  "results": [
    {
      "id": 0,
      "author": "string",
      "text": "string",
      "pub_date": "2021-10-14T20:41:29.648Z",
      "image": "string",
      "group": 0
    }
  ]
}`

- `/api/v1/posts/{post_id}/comments/ (GET, POST, PUT, PATCH, DELETE)`
- - ##### Запрос: 
`{
  "text": "string",
  "image": "string",
  "group": 0
}`

- - ##### Ответ сервера: 
`{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}`

- `/api/v1/groups/ (GET)`
- -  `[
  {
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
  }
]`

- `/api/v1/follow/ (GET, POST)`
- - `[
  {
    "user": "string",
    "following": "string"
  }
]`

## *Использованные технологии:*
<div>
<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/python/python-original.svg" title="Python" alt="Python" width="90" height="90"/>&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/django/django-plain-wordmark.svg" title="django"  alt="django" width="90" height="90"/>&nbsp;
</dev>

