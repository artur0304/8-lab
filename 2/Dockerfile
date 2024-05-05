FROM ubuntu

RUN apt-get update && apt-get -y install nginx supervisor

COPY nginx.conf /etc/nginx/nginx.conf
COPY supervisord.conf /etc/supervisord.conf

CMD ["supervisord", "-c", "/etc/supervisord.conf"]
