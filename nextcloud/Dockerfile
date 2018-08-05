FROM nextcloud:latest

RUN usermod -u 1000 www-data && groupmod -g 1000 www-data

HEALTHCHECK --interval=5m --timeout=10s CMD curl -sS -o /dev/null http://$HOSTNAME?health_check || exit 1
