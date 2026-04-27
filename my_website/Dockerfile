FROM alpine:latest

COPY . /app

WORKDIR /app

EXPOSE 80

CMD ["httpd", "-f", "-h", "/app"]