# Проект: Автоматизация учета склада носков

Этот проект представляет собой приложение для автоматизации учета носков на складе магазина. Оно позволяет кладовщику учитывать приход и отпуск носков, а также получать информацию о текущем количестве носков определенного цвета и состава.

## Основные возможности

- Регистрация прихода и отпуска носков на складе.
- Получение общего количества носков, удовлетворяющих заданным критериям.
- HTTP API для взаимодействия с приложением.

## Технологии и инструменты

- Java (версия X.X)
- Spring Boot Framework (версия X.X)
- Реляционная база данных (например, PostgreSQL)
- Liquibase (версия X.X) для управления версионированием схемы БД
- Docker для контейнеризации приложения и базы данных
- Облачный сервис (например, Heroku) для развертывания приложения и доступа к его API

## Использование API
Примеры запросов к API:

Зарегистрировать приход носков:

POST /api/socks/income
{
  "color": "red",
  "cottonPart": 95,
  "quantity": 50
}

Зарегистрировать отпуск носков:

POST /api/socks/outcome
{
  "color": "black",
  "cottonPart": 5,  
  "quantity": 10
}

Получить общее количество носков:

GET /api/socks?color=red&operation=moreThan&cottonPart=90

## Вклад и обратная связь
Если вы хотите внести свой вклад в развитие этого проекта, вы можете создать pull request. Если у вас есть какие-либо вопросы или предложения, пожалуйста, создайте issue.
