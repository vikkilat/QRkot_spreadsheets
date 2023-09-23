# Приложение для Благотворительного фонда поддержки котиков QRKot

Фонд собирает пожертвования на различные целевые проекты: на медицинское обслуживание нуждающихся хвостатых, на обустройство кошачьей колонии в подвале, на корм оставшимся без попечения кошкам — на любые цели, связанные с поддержкой кошачьей популяции.

## Стек технологий:

* Python 3.9.10
* FastAPI
* SQLAlchemy
* Google API

## Как запустить проект:

* Клонировать репозиторий:

```
git clone git@github.com:vikkilat/QRkot_spreadsheets.git
```

* Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/Scripts/activate
```

* Установить зависимости из файла ```requirements.txt```:

```
pip install -r requirements.txt
```

* Выполнить миграции:
```
alembic init --template async alembic
alembic revision --autogenerate -m "migration name"
alembic upgrade head
```

* Запустить проект локально:
```
uvicorn app.main:app --reload
```

## Автор:
[Латышева Виктория](https://github.com/vikkilat)
