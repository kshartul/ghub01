FROM nginx:1.19-alpine

COPY index.html /usr/share/nginx/html/index.html

RUN apk add --no-cache ca-certificates

RUN echo "ServerName localhost" >> /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]