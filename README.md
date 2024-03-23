# Инструкции по запуску приложение с помощью DOCKER

## Задачи

- Опишите Dockerfile для запуска контейнера с проектом.
- Оберните в Docker Compose Django-проект с БД PostgreSQL.
- Допишите в docker-compose.yaml работу с Redis.
- Допишите в docker-compose.yaml работу с Celery.

### Краткая справка

Поддерживается :
сообществом Docker PostgreSQL, REDIS.

Где получить помощь :
Slack сообщества Docker , Server Fault , Unix и Linux или Stack Overflow.

### PostgreSQL

Куда сообщать о проблемах :
https://github.com/docker-library/postgres/issues .

Поддерживаемые архитектуры : ( подробнее )
amd64, arm32v5, arm32v6, arm32v7, arm64v8, i386, mips64le, ppc64le,s390x

Сведения об артефакте опубликованного изображения : каталог репозитория
repo-inforepos/postgres/ ( история )
(метаданные изображения, размер передачи и т. д.).

Обновления изображений : метка
репозитория официальных изображений library/postgresФайл
репозитория официальных изображенийlibrary/postgres ( история )

Источник этого описания : каталог
репозитория документовpostgres/ ( история ).

### REDIS

Куда сообщать о проблемах :
https://github.com/docker-library/redis/issues .

Поддерживаемые архитектуры : ( подробнее )
amd64, arm32v5, arm32v6, arm32v7, arm64v8, i386, mips64le, ppc64le,s390x

Сведения об артефакте опубликованного изображения : каталог репозитория
repo-inforepos/redis/ ( история )
(метаданные изображения, размер передачи и т. д.).

Обновления изображений : метка
репозитория официальных изображений library/redisФайл
репозитория официальных изображенийlibrary/redis ( история )

Источник этого описания : каталог
репозитория документовredis/ ( история ).

### Как запустить проект с помощью Docker-compose:

В терминале набираем команду

        docker-compose build

docker-compose build — позволяет обновить образы или создать их заново, если они были изменены;

Далее набираем команду

        docker-compose up

docker-compose up — запускает приложение со всеми контейнеры, информация о которых есть в docker-compose.yml. Если файл
не указан, по умолчанию используется файл в текущем каталоге

Остальные команды для DOCKER которыми вы можете воспользоваться в своем проекте.

        docker-compose restart

Docker-compose restart — перезапускает контейнеры;

        docker-compose logs

Docker-compose logs — выводит журналы состояния;

        docker-compose ps

Docker-compose ps — отображает текущее состояние контейнеров.

        docker-compose down

Docker-compose down — останавливает и удаляет все контейнеры, а также тома, связанные с ними.

        docker-compose start

Docker-compose start — запускает остановленные контейнеры.

        docker-compose stop

Docker-compose stop — останавливает работу запущенных контейнеров без их удаления.

        docker-compose restart

Docker-compose restart — перезапускает контейнеры.

        docker-compose pull

Docker-compose pull — загружает последние версии образов для сервисов, описанных в файле docker-compose.yml