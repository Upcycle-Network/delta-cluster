FROM FROM alpine:3.20
RUN apk add --no-cache lighttpd
COPY lighttpd.conf /etc/lighttpd/lighttpd.conf
COPY ./index.html /var/www/html/
EXPOSE 80
CMD ["lighttpd", "-D", "-f", "/etc/lighttpd/lighttpd.conf"]