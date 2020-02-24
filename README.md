# Zoneminder 1.30.4 for Raspberry Pi

To run:
```
sudo docker build github.com/rwagnervm/rpi-zoneminder -t rwagnervm/rpi-zoneminder

sudo docker run -d -e TZ="America/Fortaleza" --restart=always --privileged="true" -p 8080:80 --name zoneminder -v "/usr/share/hassio/share/zoneminder/config":"/config":rw -v "/usr/share/hassio/share/zoneminder/data":"/var/cache/zoneminder":rw rwagnervm/rpi-zoneminder
```
