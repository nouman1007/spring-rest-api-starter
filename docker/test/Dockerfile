FROM php:8.3.0alpha1-cli-alpine3.18

COPY docker_test.sh /docker_test.sh

RUN set -ex; \
    chmod 755 /docker_test.sh; \
    apk add --update \
        curl \
        git \
    ; \
    \
    rm -rf /var/cache/apk/*

CMD ["/docker_test.sh"]
