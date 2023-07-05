FROM debian:buster

COPY conf/nginx.conf /tmp/nginx.conf
COPY tools/script.sh /tmp/script.sh

RUN chmod +x /tmp/script.sh
RUN /tmp/script.sh

EXPOSE 443

CMD [ "nginx", "-g", "daemon off;" ]