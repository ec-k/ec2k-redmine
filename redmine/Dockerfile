FROM redmine:5.0.5

ENV REDMINE_DB_MYSQL mysql
ENV TZ Asia/Tokyo

COPY plugins /usr/src/redmine/plugins
COPY themes /usr/src/redmine/public/themes
COPY config/configuration.yml /usr/src/redmine/config/