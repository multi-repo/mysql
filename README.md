### Start example

#### Default start 

```
podman run --name mysql -p 3306:3306 ghcr.io/multi-repo/mysql/mysql:main
```
if default start using url:
``` mysql://myuser:mypassword@127.0.0.1:3306/mydatabase ```

### Custom start (linux, mac os)

```
podman run \
  --name mysql \
  -e MYSQL_ROOT_PASSWORD=rootpassword \
  -e MYSQL_DATABASE=mydatabase \
  -e MYSQL_USER=myuser \
  -e MYSQL_PASSWORD=mypassword \
  -p 3306:3306 \
  ghcr.io/multi-repo/mysql/mysql:main
```

### Custom start (powershell)
```
podman run `
  --name mysql `
  -e MYSQL_ROOT_PASSWORD=rootpassword `
  -e MYSQL_DATABASE=mydatabase `
  -e MYSQL_USER=myuser `
  -e MYSQL_PASSWORD=mypassword `
  -p 3306:3306 `
  ghcr.io/multi-repo/mysql/mysql:main
```

#### Url format
`mysql://[user]:[password]@[host]:[port]/[database]`
