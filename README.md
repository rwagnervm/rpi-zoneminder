# Zoneminder 1.30.4 for Raspberry Pi

To run:
```
docker build github.com/rwagnervm/rpi-zoneminder -t rwagnervm/rpi-zoneminder

docker run -d -e TZ="America/Fortaleza" --restart=always --privileged="true" -p 8080:80 --name zoneminder -v "/opt/zoneminder/config":"/config":rw -v "/opt/zoneminder/data":"/var/cache/zoneminder":rw rwagnervm/rpi-zoneminder
```
