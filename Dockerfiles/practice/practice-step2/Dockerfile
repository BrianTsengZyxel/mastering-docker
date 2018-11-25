FROM python:alpine

COPY web /web

RUN apk add redis && \
    pip install Flask Redis

CMD ["sh", "/web/run-service.sh"]