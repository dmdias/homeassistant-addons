FROM docker.elastic.co/elasticsearch/elasticsearch:7.17.3

RUN ./bin/elasticsearch-plugin install analysis-icu
RUN ./bin/elasticsearch-plugin install analysis-kuromoji
RUN ./bin/elasticsearch-plugin install analysis-smartcn
RUN ./bin/elasticsearch-plugin install analysis-stempel

EXPOSE 9200 9300
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
CMD ["eswrapper"]

ENV HEALTH_PORT="9200" \
    HEALTH_URL=""
HEALTHCHECK \
    --interval=5s \
    --retries=5 \
    --start-period=30s \
    --timeout=25s \
    CMD curl --fail "http://127.0.0.1:${HEALTH_PORT}${HEALTH_URL}" &>/dev/null || exit 1