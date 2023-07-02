#  kittygram_final

_eng_

### Project Description
The social network is at a minimum, with the possibility of publishing photos of cats and their achievements.

### A note from a project using Docker hub
To launch, it is not necessary to create a project folder, download kittygram and transfer it to it:

``
mkdir kittygram kittygram
CD
```

In the project folder, download the docker-compose.production.yml file and upload it:

`sudo docker compose -f docker-compose.production.yml up`

Images will be downloaded, containers will be created and enabled, volumes and networks will be created.

### Subscribe to the project from sources on GitHub

Clone a repository for ourselves:

`git clone <required repository>`

Performing the launch:

`sudo docker compose -f docker-compose.yml up`

### After launch: Migrations, statistics collection

After the launch, it is necessary to collect statistics and migrate the backend. Frontend statistics are collected during container startup, after which it stops.

``
sudo docker compose -f [filename-docker-compose.yml] executes the python backend manage.py migrate

sudo docker compose -f [filename-docker-compose.yml] executes the python backend manage.py static collection

sudo docker compose -f [filename-docker-compose.yml] executes the cp -r /app/collected_static/ server part. /static/static/
``

### Stop the container orchestra

`sudo docker compose -f docker-compose.yml is disabled`

### Technologies
- _Python 3.9_
- _Django 3.2.3_
- _Django REST framework 3.12.4_
- _JavaScript_
- _doker_


### Author

_Bogatyrev Roman_

____

_рус_

### Описание проекта
Социальная сеть на минимуме, с возможностью публикации фотографий котиков и их достижений.

### Запуск проекта из образов с Docker hub
Для запуска необходимо на создать папку проекта, например kittygram и перейти в нее:

```
mkdir kittygram
cd kittygram
```

В папку проекта скачиваем файл docker-compose.production.yml и запускаем его:

`sudo docker compose -f docker-compose.production.yml up`

Произойдет скачивание образов, создание и включение контейнеров, создание томов и сети.

### Запуск проекта из исходников GitHub

Клонируем себе репозиторий:

`git clone <необходимый_репозиторий>`

Выполняем запуск:

`sudo docker compose -f docker-compose.yml up`

### После запуска: Миграции, сбор статистики

После запуска необходимо выполнить сбор статистики и миграции бэкенда. Статистика фронтенда собирается во время запуска контейнера, после чего он останавливается.

```
sudo docker compose -f [имя-файла-docker-compose.yml] exec backend python manage.py migrate

sudo docker compose -f [имя-файла-docker-compose.yml] exec backend python manage.py collectstatic

sudo docker compose -f [имя-файла-docker-compose.yml] exec backend cp -r /app/collected_static/. /static/static/
```

### Остановка оркестра контейнеров

`sudo docker compose -f docker-compose.yml down`

### Технологии
- _Python 3.9_
- _Django 3.2.3_
- _Django REST framework 3.12.4_
- _JavaScript_
- _Docker_


### Автор

_Богатырев Роман_
