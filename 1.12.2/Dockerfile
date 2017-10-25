FROM alpine:3.6
MAINTAINER Ling <x@e2.to>
ENV NGINX_VERSION=1.12.2

RUN apk add --update nginx=${NGINX_VERSION}-r0 ca-certificates bash && \
    rm -rf /tmp/* /var/cache/apk/*

COPY config/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80 443

CMD ["nginx"]

# EOF
