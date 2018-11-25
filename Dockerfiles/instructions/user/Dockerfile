FROM alpine

RUN addgroup -S app && adduser -S appuser app

USER appuser

CMD [ "id", "-u", "-n" ]