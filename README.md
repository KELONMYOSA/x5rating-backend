# OpinioNet - Сервис анализа отзывов

## Связанные репозитории

- [**Parser**](https://github.com/KELONMYOSA/x5rating-yandex-maps-parser)
- [**Backend**](https://github.com/KELONMYOSA/x5rating-backend)
- [**Frontend**](https://github.com/KELONMYOSA/x5rating-frontend)

## :page_with_curl: Содержание

➠ [Технологический стек](#computer-технологический-стек)

➠ [Запуск приложения](#technologist-запуск-приложения)

➠ [Скриншоты](#bar_chart-скриншоты)

## :computer: Технологический стек

<p align="center">
<img width="5%" title="Playwright" src="images/logo/Playwright.svg">
<img width="5%" title="Clickhouse" src="images/logo/ClickHouse.svg">
<img width="5%" title="FastAPI" src="images/logo/FastAPI.svg">
<img width="6%" title="Docker" src="images/logo/Docker.svg">
<img width="6%" title="Nginx" src="images/logo/Nginx.svg">
<img width="6%" title="Deno" src="images/logo/Deno.svg">
<img width="6%" title="Preact" src="images/logo/Preact.svg">
</p>

**Parser**

> В качестве библиотеки для взаимодействия с Chrome используется <code>Playwright</code>.
> 
> Полученные данные отправляются в NoSQL базу данных <code>ClickHouse</code>.

**Backend**

> <code>FastAPI</code> используется для создания API-сервера со встроенной валидацией, сериализацией и асинхронностью.

**Frontend**

> Веб-сервер <code>Nginx</code> балансирует нагрузки, что повышает отказоустойчивость сервера.
> 
> В проекте используется фреймворк <code>Fresh</code> для <code>Deno</code>, который использует островную архитектуру.
> 
> <code>Fresh</code> по умолчанию использует <code>Preact</code>, который позволяет создавать интерактивные пользовательские интерфейсы с использованием реактивной модели программирования.

## :technologist: Запуск приложения

### Переменные окружения


```
CLICKHOUSE_HOST - Адрес сервера, где находится база данных
CLICKHOUSE_USERNAME - Имя пользователя Clickhouse
CLICKHOUSE_PASSWORD - Пароль Clickhouse
```

### Запуск в Docker

**Backend**

Сборка образа из Dockerfile - <code>docker compose build --no-cache</code>

Запуск контейнеров - <code>docker compose up -d</code>

**Frontend**

Запуск контейнеров - <code>docker compose up -d</code>

## :bar_chart: Скриншоты

> На данной странице отображаются карточки магазинов с ключевыми характеристиками из отзывов

<p align="center">
  <img src="images/Screenshot_1.png">
</p>

> Адаптивная верстка для мобильных устройств

<p align="center">
  <img src="images/Screenshot_2.png">
</p>
