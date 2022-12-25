# Проект «API для Yatube» спринт №9 в рамках учебного курса Яндекс.Практикум

## Описание
API для социальной сети блогеров Yatube, созданной в рамках учебного курса Яндекс.Практикум
API - это интерфейс для обмена данными, предоставляет доступ к постам, комментариям, группам и подпискам Yatube,
в зависимости от статуса пользователя. Аутентификация реализована по JWT - токену.

## возможности
- Получение постов для любых пользователей
- Написание постов для авторизированных пользователей
- Разбиение постов на группы
- Получение и работа с комментариями к постам
- Подписка на авторов

## Технологии
Python 3.7
djangorestframework 3.12.4

## Запуск проекта
- Клонируйте репозитроий с проектом:
```
git clone
```
- Установите и активируйте виртуальное окружение
```
python -m venv venv
```
- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- Выполните миграции:
```
cd yatube_api
manage.py migrate
```
- Запустить серевер, выполнив команду:
```
python manage.py runserver
```

## Примеры запросов к API.
- Получить список всех публикаций
```
GET /api/v1/posts/
```
- Получение публикации по id.
```
GET /api/v1/posts/{id}/
```
- Получение комментария к публикации по id.
```
GET /api/v1/posts/{post_id}/comments/{id}/
```

## Авторы
Дмитрий 