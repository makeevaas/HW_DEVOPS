FROM alpine:latest

RUN apk update && apk upgrade

RUN apk add nginx

COPY nginx.conf /etc/nginx/server/nginx.conf

EXPOSE 80/tcp

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
