FROM alpine:3.6
MAINTAINER e2tox@live.com
ENV NGINX_VERSION=1.12.1-r0
RUN apk upgrade --update && \
    apk add --update nginx=${NGINX_VERSION} ca-certificates bash && \
    rm -rf /tmp/* /var/cache/apk/*

COPY config/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80 443

CMD ["nginx"]

# EOF
