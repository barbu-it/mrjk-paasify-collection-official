# Home Assistant

## Create mqtt user

See: https://techoverflow.net/2021/11/25/how-to-setup-standalone-mosquitto-mqtt-broker-using-docker-compose/

```
docker-compose exec mosquitto mosquitto_passwd -c /mosquitto/conf/mosquitto.passwd mosquitto
docker-compose exec mosquitto mosquitto_passwd -b /mosquitto/conf/mosquitto.passwd seconduser PASSWORD
```

Better: cd into mqtt config
```
touch mosquitto.passwd
docker run --rm -it -v $PWD:/work/ eclipse-mosquitto mosquitto_passwd /work/mosquitto.passwd  admin
docker run --rm -it -v $PWD:/work/ eclipse-mosquitto mosquitto_passwd -b /work/mosquitto.passwd  domotic domotic
```

