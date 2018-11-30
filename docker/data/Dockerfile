FROM alpine:3.7

RUN apk add --no-cache \
    bash \
    zip

# Добавляем PHP-исходники нашего веб приложения
ADD app /app

COPY docker/data/docker-entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]