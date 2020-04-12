FROM nginx

RUN apt-get update
RUN apt-get install -y geoip-database libgeoip1

COPY ./conf.d/web.conf /etc/nginx/conf.d/web.conf
COPY ./nginx.conf /etc/nginx/nginx.conf 

CMD ["nginc", "-g", "daemon off;"]