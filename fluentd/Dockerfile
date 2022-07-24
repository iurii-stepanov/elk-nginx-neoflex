# fluentd/Dockerfile
FROM fluentd:v1.14-1
USER root
RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-document"]
COPY ./conf/fluent.conf /fluentd/etc/
USER fluent