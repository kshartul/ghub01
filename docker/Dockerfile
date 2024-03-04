FROM nginx:1.19-alpine

RUN apk update && apk add git
RUN apk add --no-cache ca-certificates

COPY /webpage/index.html /usr/share/nginx/html/index.html
RUN echo "ServerName localhost" >> /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]