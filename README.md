# API Yatube
### Описание проекта.
Проект представляет собой сервис для блогеров, в котором каждый зарегистрированный пользователь может создавать посты и комментировать их, подписываться на понравившихся авторов.
Настоящий репозиторий - API для данного проекта.

##### Технологии.
В проекте использованы следующие технологии:
Python 3.7, Django 2.2.16, Django REST Framework, JWT (JSON Web Token), Djoser.
### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/mdkostrov/api_final_yatube.git
```

```
cd yatube_api
```

Cоздать и активировать виртуальное окружение (для Windows):

```
python -m venv env
```

```
source venv/scripts/activate
```

Обновить установщик пакетов pip:

```
python -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции (для Windows):

```
python manage.py migrate
```

Запустить проект (для Windows):

```
python manage.py runserver
```

### Пример запросов к API:
GET-запрос к эндпоинту

```
/api/v1/posts/
```

Вернет список записей.

При указании параметров limit и offset:
```
/api/v1/posts/?limit=2&offset=4
```
ответ будет с соответствующей постраничной разбивкой.


### Документация
Документация с остальными доступными для запросов эндпоинтами после запуска DEV-сервера проекта доступна по адресу:

```
http://127.0.0.1:8000/redoc/
```

### Об авторе:
Автор проекта: **Костров Михаил**.
Студент курса "Разработчик Python" (45-47 когорт).
* [GitHub](https://github.com/mdkostrov/)
* [Telegram](https://t.me/MihaMaha)
* [VK](https://vk.com/mdkostrov)
