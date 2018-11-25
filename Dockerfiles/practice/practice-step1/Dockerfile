FROM python:alpine

COPY web /web

RUN apk add redis

RUN pip install Flask Redis

CMD ["sh", "/web/run-service.sh"]