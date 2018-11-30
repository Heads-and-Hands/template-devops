FROM nginx

# Добавляем PHP-исходники нашего веб приложения
#ADD app /var/www/app

# Добавляем наш конфиг
ADD docker/nginx/conf/default.conf /etc/nginx/conf.d/default.conf

CMD /bin/bash -c "exec nginx -g 'daemon off;'"