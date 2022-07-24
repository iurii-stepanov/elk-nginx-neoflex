# fluentd/Dockerfile
FROM fluentd:v1.14-1
USER root
RUN ["gem", "uninstall", "-I", "elasticsearch"]
RUN ["gem", "install", "elasticsearch", "-v", "7.17.0"]
RUN ["gem", "install", "fluent-plugin-elasticsearch"]
COPY ./conf/fluent.conf /fluentd/etc/
USER fluent