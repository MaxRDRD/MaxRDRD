# Привет, я Максим 👋
 
**Backend-разработчик на Go.** Студент 3 курса, программная инженерия.
Ищу стажировку или позицию junior Go-разработчика.
 
Делаю backend-сервисы с понятной архитектурой и тестами: проектирую API, работаю с PostgreSQL и Kafka, упаковываю всё в Docker.
 
## Стек
 
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
 
## Проекты
 
### [Top Queries Service](https://github.com/MaxRDRD/Internship_wb_tech)
Сервис читает поисковые события из Kafka и отдаёт Top-N самых частых запросов за последние 5 минут.
- Скользящее окно из 300 секундных бакетов в памяти: запись за O(1), осознанный компромисс «дешёвая запись, дорогое чтение»
- Стоп-лист, который применяется без перезапуска, и антиспам-лимит на сессию и пользователя
- Слоистая архитектура (domain / usecase / ports / adapters), unit-тесты, запуск через Docker Compose вместе с Kafka
`Go` `Kafka` `Docker`
 
### [RoomBooking](https://github.com/MaxRDRD/RoomBooking)
Сервис бронирования переговорок.
- JWT-авторизация с ролями admin и user, расписания переговорок, ленивое формирование слотов, создание и идемпотентная отмена броней, пагинация
- Защита от двойного бронирования на уровне ограничения в БД
- OpenAPI-спецификация, unit- и e2e-тесты, golangci-lint, CI, запуск одной командой через docker compose
`Go` `PostgreSQL` `chi` `pgx` `Docker`
 
### [SmartRun](https://github.com/MaxRDRD/Portfolio_SmartRun)
Pet-проект: аналитика бега. Импортирует `.fit`-файлы, считает нагрузку и готовность (TSS, CTL/ATL/TSB), а рекомендацию на день формирует Google Gemini.
- Backend на Go (chi, pgx): JWT, TOTP 2FA, rate limiting, фоновые воркеры на RabbitMQ
- PostgreSQL с миграциями, Redis-кэш с circuit breaker, запуск одной командой через Docker Compose
- Веб-интерфейс на чистом HTML/CSS/JS
`Go` `PostgreSQL` `Redis` `RabbitMQ` `Docker`
 
## Контакты
 
📧 max.rusin37@gmail.com

 
