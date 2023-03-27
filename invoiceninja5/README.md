# Invoice Ninja


## Reset password account

To generate a new password hash, go into app container:
```
php artisan tinker
bcrypt('new password');
```

To change account password in DB, go into DB container:
```
mysql -p${MYSQL_ROOT_PASSWORD}
> use invoiceninja5
> update users set password = "NEW_HASH" where email = "user@domain.com" ;

```
