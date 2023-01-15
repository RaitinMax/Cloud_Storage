# [Дипломная работа “Облачное хранилище”](https://github.com/netology-code/jd-homeworks/blob/master/diploma/cloudservice.md)


## Стартовые пользователи:

**USERNAME:** user@one.user **PASSWORD:** user_one

**USERNAME:** user@two.user **PASSWORD:** user_two

## Запуск приложения

### Запуск BACKEND:

1. Скачать данный проект, выполнить `maven -> clean -> package`;
2. Запустить `docker-compose.yml`.
Автоматически создадутся все необходимые в базе данных таблицы (с двумя стартовыми пользователями в таблице users).

BACKEND можно запустить и через main метод в классе NetologyCloudStorageApplication.java,
не используя docker-контейнер. Базу данных же все равно запускать через docker-контейнер.

Для этого на п.2 "Запуск BACKEND" вместо запуска всего `docker-compose.yml` следует запустить
только `docker-compose.yml -> database`, а само приложение через main метод.
Остальные шаги остаются неизменны.
