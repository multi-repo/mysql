### Start example

```
podman run \
  --name mysql \
  -e MYSQL_ROOT_PASSWORD=rootpassword \
  -e MYSQL_DATABASE=mydatabase \
  -e MYSQL_USER=myuser \
  -e MYSQL_PASSWORD=mypassword \
  -p 3306:3306 \
  bitnami/mysql:latest
```

```
mysql://myuser:mypassword@127.0.0.1:3306/mydatabase
```
