# docker-cleanup

```
    # remove some containers
    docker ps -a | grep -v CONTAINER | awk '{print $1}' | xargs docker rm
```

```
    # remove some images
    docker images | grep -v REPOSITORY | awk '{print $3}' | xargs docker rmi
```
