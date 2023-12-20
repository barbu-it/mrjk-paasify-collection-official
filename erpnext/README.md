# ERPNext


## Quickstart

Paasify example:
```
  - app: official:erpnext
    vars:
      app_admin_pass: admin
      app_db_pass: 123
      app_db_admin_pass: 456
    tags:
      - mariadb
      - redis
      - traefik-svc
      - homepage
```

Then you have a fresh website generator.

```
docker compose --project-name jez_beta_erpnext --file ../erpnext/docker-compose.run.yml run  backend bench new-site erpnext.beta.jeznet.org --no-mariadb-socket --mariadb-root-password $app_db_root_pass  --admin-password admin123
```


Note:
you may need to create apps.txt and site commmon

