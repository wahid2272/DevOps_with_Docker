## Solution of task 1.9

```console
touch /tmp/log.txt
````

```console
docker run -v ${pwd}/tmp/log.txt:/usr/app/logs.txt devopsdockeruh/simple-web-service
```
