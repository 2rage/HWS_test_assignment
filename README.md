# HWSchool test

## Тестовое задание для hwschool

- **/tgbot** - первое задание
- **/superheroapp** - второе задание

## Первое задание

### Структура приложения:

```bash
tgbot/
│
├── app/
│   ├── __init__.py          # Инициализация приложения и его компонентов
│   ├── config.py            # Конфигурационные настройки бота
│   ├── handlers.py          # Функции обработки сообщений и команд
│   ├── models.py            # Описание моделей данных
│   └── routes.py            # Маршруты и регистрация обработчиков сообщений
└── run.py                   # Запуск приложения
```

**Для запуска приложения используйте**: `run.py`

### Пример работы приложения:

<img src="/images/image.png" width="650">
<img src="/images/image-1.png" width="650">
<img src="/images/image-2.png" width="650">
<img src="/images/image-3.png" width="650">


## Второе задание:

Переписал приложение на Flask с использованием SQLAlchemy. 
- Исправил некорректное отображение героев с ростом выше 180см и силой более 80
- Скорректировал запрос на отображение средних значений по полу
- Упаковал приложение для простоты запуска через `run.py`
- Скорректировал первоначальный запуск приложения и заполнения базы данных в случае обрыва соединения
- Настроил сессии и добавил функцию для кнопки экспорта в CSV. 

### Структура приложения:

```bash
superheroapp/
│
├── app/
│   ├── __init__.py          # Инициализация Flask приложения
│   ├── models.py            # Описание моделей SQLAlchemy
│   ├── routes.py            # Маршруты приложения
│   └── database.py          # Настройка базы данных
└── run.py                   # Запуск приложения Flask
```

**Для запуска приложения используйте**: `run.py`

### Пример работы приложения:

<img src="/images/image-8.png" width="650">
<img src="/images/image-9.png" width="650">
<img src="/images/image-10.png" width="650">
<img src="/images/image-11.png" width="650">
<img src="/images/image-12.png" width="650">
<img src="/images/image-13.png" width="650">
<img src="/images/image-14.png" width="650">


## Старая функциональность:

- **/codetest/initbd.py** - инициализация и создание БД
- **/codetest/bdcomplete.py** - заполнение БД с помощью superheroAPI
- **/codetest/create_csv_files.py** - вывод данных из БД в CSV формате
- **tall_strong_heroes.csv** - герои с ростом более 180 и силой больше 80
- **avg_by_gender.csv** - средние значения по полу
- **top_strength.csv** - ТОП-5 супергероев по силе

В ветке [v2](https://github.com/2rage/HWS_test_assignment/tree/v2) реализовал небольшое Flask-приложение, которое выводит данные таблиц через веб-интерфейс. Для оформления использовал Bootstrap.

Запуск приложения - `python3 create_csv_files.py`

#### Пример работы приложения:

<img src="/images/image-4.png" width="800">
<img src="/images/image-5.png" width="800">
<img src="/images/image-6.png" width="800">
<img src="/images/image-7.png" width="800">