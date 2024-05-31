# Docker

Containers are meant to run a specific task or process.

## Commands

docker ps -a

docker images

docker build webapp-color -t webapp-color:tag

docker run -p 8282:8080 webapp-color  (host port:container port)

docker run -e APP_COLOR=pink simpleapp

docker run -it python:3.6 sh

cat /etc/resolv.conf - system version

## Dockerfile

CMD ["executable", "param1"] or CMD executable param1

CMD allows to set a default command which can be overriden by `docker run ubuntu [COMMAND]` for example `docker run ubuntu sleep 5`

ENTRYPOINT specifies a program that will be run at startup.

When overriding CMD is replaced and ENTRYPOINT stays and appends args.

```Dockerfile
FROM Ubuntu

ENTRYPOINT ["sleep"]

CMD ["5"]
```

docker run ubuntu-sleeper -> sleep 5
docker run ubuntu-sleeper 10 -> sleep 10
docker run --entrypoint sleep2.0 ubuntu-sleeper 10 -> sleep2.0 10

## Security

ps aux - processes

docker run --user=1000 ubuntu sleep 3600 - run as user

or in Dockerfile `USER 1000`

System privileges can be added/removed with `docker run --cap-add MAC_ADMIN ubuntu` and `docker run --cap-drop KILL ubuntu.

Container can be run with all privileges with `docker run --privileged ubuntu`.
