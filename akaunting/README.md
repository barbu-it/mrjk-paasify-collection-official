# Akaunting

See: https://github.com/akaunting/docker

## Quickstart

For the first start, you must start the copntainer with: `AKAUNTING_SETUP: true` and create artiusan modules

Also: https://github.com/akaunting/docker/issues/53#issuecomment-1033379921
```
$ docker create --name akaunting-tmp akaunting/akaunting
eb0ee9382ed422c56b8ba00ec3dfebac1bb57bb854ceca989d4d31fd2c37b5e8
$ docker cp akaunting-tmp:/var/www/html/modules/. ./plugins/
$ docker rm akaunting-tmp
akaunting-tmp
```


Note: For now, jsut patch temporarly `docker-compose.run.yml` for AKAUNTING_SETUP=true (true must be in lowercase)

You need the to connect with: ADMIN_EMAIL/ADMIN_PASSWORD
