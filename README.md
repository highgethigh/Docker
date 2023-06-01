Настройка Django + Gunicorn, PostgreSQL, NginX.

`docker-compose up -d`

`docker-compose up --build -d`



## Обновление баз данных
`docker-compose exec djangoapp python /djangoapp/manage.py makemigrations`
`docker-compose exec djangoapp python /djangoapp/manage.py migrate`

## Создаем пользователя в админке
`docker-compose exec djangoapp python /djangoapp/manage.py createsuperuser`

## Переходим на сервер
Server: http://localhost:8000/

## Далее в админку 
http://localhost:8000/admin/
User:<b>admin</b>
Password:<b>admin</b>
