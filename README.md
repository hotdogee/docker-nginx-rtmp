# docker-nginx-rtmp
A Dockerfile installing NGINX, nginx-rtmp-module and FFmpeg from source with
default settings for HLS live streaming. Built on Alpine Linux.

* Nginx 1.17.1 (Stable version compiled from source)
* nginx-rtmp-module master (compiled from source)
* ffmpeg 4.1.4 (compiled from source)

## Usage

* Build and run container from source:
```
docker build -t nginx-rtmp .
docker run -it -p 1935:1935 -p 8085:80 --rm nginx-rtmp
```
