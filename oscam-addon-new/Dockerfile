# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
#FROM linuxserver/oscam:latest
ARG BUILD_FROM
FROM $BUILD_FROM

# Set environment variables
ENV PUID=1000 \
    PGID=1000 \
    TZ=Etc/UTC

#EXPOSE 8888 9000