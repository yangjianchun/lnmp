ARG NGINX_VERSION=latest
FROM nginx:${NGINX_VERSION}

LABEL maintainer="yjc-nginx"

COPY nginx.conf /etc/nginx/

ARG CHANGE_SOURCE=false
RUN if [ ${CHANGE_SOURCE} = true ]; then \
    # Change application source from dl-cdn.alpinelinux.org to aliyun source
    sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/' /etc/apk/repositories \
;fi

RUN apk update \
    && apk upgrade \
    && apk add --no-cache bash \
    && adduser -D -H -u 1000 -s /bin/bash www-data
    
CMD ["nginx"]

EXPOSE 80 443
