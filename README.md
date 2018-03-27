# dvdisaster

Containerised version of [dvdisaster](http://www.dvdisaster.com/en/index.html)

dvdisaster is a tool for ensuring your optical media is recoverable and is able to test the readability of discs.

Based on the brilliant [jlesage/docker-baseimage-gui](https://github.com/jlesage/docker-baseimage-gui)

---
#### 0.0.1

- 2018-03-26 :: Initial release

---
#### Example Run Command

```
docker run -it --rm \
  -p 5820:5800 \
  -e KEEP_APP_RUNNING=1 \
  -e DISPLAY_WIDTH=1280 \
  -e DISPLAY_HEIGHT=768 \
  -v /srv/archiving:/data \
  --device=/dev/sr0 \
  b3vis/dvdisaster
```
