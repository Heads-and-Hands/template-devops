FROM alpine:3.7

RUN apk add --no-cache \
    bash \
    zip

# Добавляем PHP-исходники нашего веб приложения
ADD app /app

# Даем права на файлы для сервера
RUN chmod -R 777 /app/web/runtime
RUN chmod -R 777 /app/web/files

COPY docker/data/docker-entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
