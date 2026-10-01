# СКАНФЛИТ — Dockhost

Статический сайт на HTML, запускаемый в Docker через Nginx.

## Локальная проверка

```bash
docker build -t skanfleet-site .
docker run --rm -p 8080:80 skanfleet-site
```

Откройте http://localhost:8080

## Dockhost

Создайте проект и приложение/контейнер из Git-репозитория или Docker-образа согласно интерфейсу Dockhost.

Если Dockhost собирает Dockerfile из репозитория, оставьте Dockerfile в корне проекта.

Контейнер слушает порт 80.

После запуска добавьте сетевой сервис/маршрут на порт 80 и привяжите домен в разделе сетевых сервисов Dockhost.
