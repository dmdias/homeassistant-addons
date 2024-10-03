
ARG BUILD_FROM
FROM $BUILD_FROM

RUN apk update && apk add --no-cache \
    build-base \
    cmake \
    git \
    curl \
    && curl -L https://github.com/oscam-emu/oscam/archive/master.tar.gz | tar xz \
    && cd oscam-master \
    && cmake . && make && make install

EXPOSE 8888 9000

COPY run.sh /run.sh
RUN chmod +x /run.sh

CMD [ "/run.sh" ]