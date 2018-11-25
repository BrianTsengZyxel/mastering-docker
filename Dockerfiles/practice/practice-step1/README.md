#   Dockerfile practice

##  Web Page

![](../images/web.png)

##  Base image

*   [python:alpine](https://hub.docker.com/_/python/)

##  Steps

1.  Install redis and openrc
    ```
    apk add redis openrc
    ```

2.  Enable redis service at boot time
    ```
    rc-update add redis
    ```

3.  Install python packages (Flask & Redis) by pip
    ```
    pip install Flask Redis
    ```

4.  Copy the web python file to container

5.  Start the redis service on daemon mode
    ```
    redis-server --daemonize yes
    ```

6.  Start the web page (Listen port: `80`)
    ```
    python app.py
    ```
