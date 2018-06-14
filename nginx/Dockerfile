FROM nginx:alpine

RUN set -x ; \
  addgroup -g 82 -S www-data ; \
  adduser -u 82 -D -S -G www-data www-data && exit 0 ; exit 1
  
RUN mkdir -p /var/run/nginx

RUN rm /etc/nginx/conf.d/default.conf

ADD conf/nginx_app.conf /etc/nginx/conf.d/nginx_app.conf
ADD conf/nginx.conf /etc/nginx/nginx.conf

WORKDIR /app
COPY www /app/www
RUN chown -R www-data:www-data /app/www