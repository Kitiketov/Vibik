# Vibik

![Platform](https://img.shields.io/badge/platform-Android-green)
![Language](https://img.shields.io/badge/language-C%23-blue)
![Framework](https://img.shields.io/badge/framework-.NET%20MAUI-purple)
![Backend](https://img.shields.io/badge/API-ASP.NET%20Core-blue)
![Status](https://img.shields.io/badge/status-in%20development-yellow)


Vibik — приложение, которое выдает задания для фотографии, чтобы люди могли отвлечься от рутины и заняться чем-то более творческим.

Этот репозиторий содержит клиентскую (frontend) часть Android-приложения.

Проект разработан в рамках учебной командной разработки.

# Contents

- [About](#about)
- [Presentation](#presentation)
- [Установка](#шаги-для-установки-vibik-пока-только-для-android)
- [Tech Stack](#tech-stack)
- [Backend](#backend)
- [Moderation panel](#moderation-panel)
- [Authors](#authors)

# About

Что можно делать в Vibik:

- получать случайные фотозадания
- выполнять задания 
- сохранять приятные моменты в истории
- просматривать выполненные задания
- развивать креативность через фотографию


# Presentation

Вот [тут](https://www.figma.com/deck/FUEbcrfThRr89p3HXibL9F) лежит презентация с нашей защиты, там можно посмореть скриншоты из приложения, метрики и много другой информации, заглядывайте ;)


# Шаги для установки vibik (пока только для android):

1. Перейдите на страницу Releases репозитория
   
2. Скачайте .apk файл приложения

3. Установите его на Android устройство

После установки вы можете запустить приложение и начать пользоваться Vibik.




# Tech Stack

### Frontend

- C#
- .NET MAUI

### Security

- JWT Bearer Authentication

### Architecture

- DDD — архитектура приложения
- ViewModel — управление состоянием UI


Основные слои приложения:

- **Core** — бизнес-логика
- **Infrastructure** — работа с API и внешними сервисами
- **Vibik** — UI и ViewModel
  

### Backend

Приложение взаимодействует с серверной частью проекта: [Vibik.Server](https://github.com/Jlychee/Vibik.Server)

Сервер реализует:

- REST API
- авторизацию пользователей
- хранение изображений
- управление заданиями

⚠️ В данный момент сервер может быть недоступен.

### Moderation panel

Приложение взаимодействует с серверной частью проекта:  [Moderation panel](https://github.com/Kitiketov/Vibik.ModeratorPanel)

Тг бот:

- отправляет уведомления модераторам
- визуализирует метрики
- отображает модерационую панель фоток
- API

⚠️ В данный момент тг бот может быть недоступен.

# Authors

- Толканюк Екатерина - проектирование и реализация REST API, работа с aws-s3 - [Jlychee](https://github.com/Jlychee)

- Скворок Артем - проектирование схемы, запросы, интеграция с PostgreSQL - [fan4cz](https://github.com/fan4cz)

- Котов Илья - реализация JWT-аутентификации, телеграм бот для модерации на aiogram + fasapi, сбор метрик - [Kitiketov](https://github.com/Kitiketov)

- Кискина Арина - дизайн, реализация пользовательского интерфейса и взаимодействия с API - [reqied](https://github.com/reqied) (это мое болото)
