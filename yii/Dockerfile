FROM nginx/unit:1.23.0-php8.0
RUN mkdir -p /opt/code
COPY code /opt/code
COPY .yii.unit.conf.json /docker-entrypoint.d/.yii.unit.conf.json
CMD ["unitd", "--no-daemon", "--control", "unix:/var/run/control.unit.sock"]