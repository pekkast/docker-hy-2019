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
```console
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

## 1.4
```console
$ docker run -d --name=bash_sample devopsdockeruh/exec_bash_exercise
$ docker exec -it bash_sample /bin/bash
root@ede7d118e3de:/usr/app# tail -f ./logs.txt
Secret message is:
"Docker is easy"
Sat, 05 Oct 2019 05:23:33 GMT
Sat, 05 Oct 2019 05:23:36 GMT
^C
root@ede7d118e3de:/usr/app# exit
$ docker stop bash_sample
$ docker rm bash_sample
$ docker rmi devopsdockeruh/exec_bash_exercise
Untagged: devopsdockeruh/exec_bash_exercise:latest
Untagged: devopsdockeruh/exec_bash_exercise@sha256:c463832132d1fb0b8b3b60348a6fc36fda7512a4ef2d1050e8bea7b6a6d7a2f3
Deleted: sha256:489b6d8f2ab81ec84032c0e16deeded4862006b787353c740f1a4659f1b28a09
Deleted: sha256:2183b84cef51c03f45122ea74e50c6a1f7f75805faa37ed02486c0543540ff52
```

## 1.5
```console
$ docker run -it ubuntu sh -c 'apt update;apt install -y curl;echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```

## 1.6
```console
$ docker build -f ./Dockerfile-1.6 -t docker-clock .
$ docker run docker-clock
```

## 1.7
```console
$ docker build -f ./Dockerfile-1.7 -t curler .

$ docker run -it curler
```
