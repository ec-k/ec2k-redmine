FROM redmine:5.0.5

ENV REDMINE_DB_MYSQL mysql
ENV TZ Asia/Tokyo

COPY config/configuration.yml /usr/src/redmine/config/

RUN apt-get update \
    && apt-get install -y --no-install-recommends git \
    && rm -rf /var/lib/apt/lists/* \
    && git clone -b redmine4.2 --depth 1 https://github.com/farend/redmine_theme_farend_bleuclair.git public/themes/bleuclair