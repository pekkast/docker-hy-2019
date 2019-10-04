## 1.1
```console
CONTAINER ID        IMAGE                        COMMAND                  CREATED              STATUS                      PORTS               NAMES
5d6a1fa221c2        nginx                        "nginx -g 'daemon of…"   About a minute ago   Exited (0) 12 seconds ago                       suspicious_heisenberg
9f27daf84f85        nginx                        "nginx -g 'daemon of…"   About a minute ago   Up About a minute           80/tcp              elated_solomon
69320ae6a77d        nginx                        "nginx -g 'daemon of…"   About a minute ago   Exited (0) 12 seconds ago                       sleepy_banzai
````

## 1.2
```console
$ docker ps -a
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
```
```bash
$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
```

## 1.3
```console
$ docker run -it devopsdockeruh/pull_exercise
Status: Downloaded newer image for devopsdockeruh/pull_exercise:latest
Give me the password: basics
You found the correct password. Secret message is:
"This is the secret message"
```