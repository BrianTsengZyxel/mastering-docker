FROM python:alpine

COPY web /web

RUN apk add --no-cache -q redis && \
    pip install -q --no-cache-dir Flask Redis

CMD ["sh", "/web/run-service.sh"]