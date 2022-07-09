# Социальная сеть Yatube

В данном проекте реализована социальная сеть для публикации личных дневников. Backend написан с помощью фреймворка Django, визуальная часть на основе HTML с использованием фреймворка Bootstrap. Код проекта покрыт Unittest-ами. 
Среди основных реализованных функций:
- Регистрация и аутентификация пользователей.
- Создание, изменение и удаление публикаций пользователем (с поддержкой статичных медиа-файлов)
- Комментирование (с возможностью редактирования и удаления) публикаций других пользователей.
- Оформление/отмена подписки на публикации других пользователей.
- Возможность добавление публикации определённой группы.
- Пагинация страниц с публикациями
- Кеширование выдачи

## Как запустить:

1. Скачать репозиторий:

```sh
git clone git@github.com:AlexeyAnanchenko/Social-Network-training-project.git
```
2. Установить и войти в виртуальное окружение:

```sh
python3 -m venv venv
```
```sh
source venv/bin/activate
```

3. Установить зависимости

```sh
pip install -r requirements.txt
```

4. Загрузить тестовые данные в базу:

```sh
sqlite3 yatube/db.sqlite < dump.sql
```

5. Запустить сервер разработчика:

```sh
python3 yatube/manage.py runserver
```


Стек:

Python 3.7
Django 2.2
Bootstrap v5