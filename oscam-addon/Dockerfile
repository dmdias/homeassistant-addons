# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
ARG BUILD_FROM
FROM $BUILD_FROM

VOLUME ["/share", "/config"]

# Set environment variables
ENV PUID=1000 \
    PGID=1000 \
    TZ=Etc/UTC