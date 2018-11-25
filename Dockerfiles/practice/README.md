#   Dockerfile practice

##  Web Page

![](web.png)

##  Base image

*   [python:alpine](https://hub.docker.com/_/python/)

##  Steps

1.  Install redis
    ```
    apk add redis
    ```

2.  Install python packages (Flask & Redis) by pip
    ```
    pip install Flask Redis
    ```

3.  Copy the web python file to container

4.  Execute the "run-service.sh"
    ```
    redis-server --daemonize yes
    python app.py
    ```
