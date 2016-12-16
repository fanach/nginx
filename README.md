# nginx

## Clone

```sh
cd /root
git clone https://github.com/fanach/share --depth=1
git clone https://github.com/fanach/nginx --depth=1
```

## Run

```sh
docker run -d --restart=always -p 80:80 -v /root/share:/home/share:ro -v /root/nginx/html:/usr/share/nginx/html:ro -v /root/nginx/nginx.conf:/etc/nginx/nginx.conf nginx:alpine
```
