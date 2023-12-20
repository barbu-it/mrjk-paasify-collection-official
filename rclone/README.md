# rclone



## Fuse mount

Use the `fuse` tag.

Source: https://forum.rclone.org/t/docker-start-rclone-automatically-with-multiple-mounts-and-webgui/20214

## Mount at startup

Example
```
mkdir -p $VOLUME_DATA/pcloud $VOLUME_DATA/dropbox $VOLUME_DATA/googledrive
docker exec rclone rclone rc options/set $AUTH --json '{"vfs": {"CacheMode": 3, "UID": '$PUID', "GID": '$PGID', "Umask": 23}, "mount": {"AllowOther": true}}'
docker exec rclone rclone rc mount/mount fs=pcloud: mountPoint=/data/pcloud $AUTH
docker exec rclone rclone rc mount/mount fs=dropbox: mountPoint=/data/dropbox $AUTH
docker exec rclone rclone rc mount/mount fs=googledrive: mountPoint=/data/googledrive $AUTH
```
