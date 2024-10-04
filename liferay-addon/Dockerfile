# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
ARG BUILD_FROM
FROM $BUILD_FROM

VOLUME ["/share", "/homeassistant_config"]

# Set environment variables
#ENV LIFERAY_JVM_OPTS=-Xms2g -Xmx2g -agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:8000 -Dcom.sun.management.jmxremote -Dcom.sun.management.jmxremote.port=9010 -Dcom.sun.management.jmxremote.local.only=false -Dcom.sun.management.jmxremote.authenticate=false -Dcom.sun.management.jmxremote.ssl=false \
#    LIFERAY_MODULE_PERIOD_FRAMEWORK_PERIOD_PROPERTIES_PERIOD_OSGI_PERIOD_CONSOLE=0.0.0.0:11311 \
#    LIFERAY_VIRTUAL_PERIOD_HOSTS_PERIOD_VALID_PERIOD_HOSTS=127.0.0.1,192.168.1.154,liferay.dmdias.info \
#    JAVA_VERSION=zulu21 \
#    LIFERAY_JPDA_ENABLED=true -e \
#    JPDA_ADDRESS=8000