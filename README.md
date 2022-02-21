# docker-images

build docker image with:

```bash
docker build ./ -t vnc-coder --no-cache
```

run a docker container with:

```bash
docker run --rm -p 6080:80 -p 5910:5900 -p 8080:8080 -e VNC_PASSWORD=password -v your-volume:/mnt/storage vnc-coder
```

* 6080 stand for noVNC
* 5910 is the port of VNC
* 8080 is code-server
