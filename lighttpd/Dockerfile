
FROM alpine:3.7

RUN apk add --no-cache lighttpd

# Create the htdocs directory and copy the HTML file into it
RUN mkdir -p /var/www/localhost/htdocs/
COPY index.html /var/www/localhost/htdocs/

EXPOSE 80

CMD ["lighttpd", "-D", "-f", "/etc/lighttpd/lighttpd.conf"]
