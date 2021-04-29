![](https://img.shields.io/badge/OS-Centos-informational?style=flat&logo=<LOGO_NAME>&logoColor=white&color=2bbc8a)
![](https://img.shields.io/badge/Nginx-informational?style=flat&logo=<LOGO_NAME>&logoColor=white&color=blue)
# nginx1.18 离线安装包
基于centos7 nginx1.18版本源码编译制作的离线安装包

## 版本说明
```
nginx版本 1.18
openssl版本: 1.1.1f
zlib版本: 1.2.11
pcre版本: 8.44
```
## Nginx 配置参数
```bash
./configure \
--prefix=/usr/local/nginx \
--pid-path=/var/run/nginx.pid \
--lock-path=/var/run/nginx.lock \
--http-client-body-temp-path=/usr/local/nginx/client_temp \
--http-proxy-temp-path=/usr/local/nginx/proxy_temp \
--http-fastcgi-temp-path=/usr/local/nginx/fastcgi_temp \
--http-uwsgi-temp-path=/usr/local/nginx/uwsgi_temp \
--http-scgi-temp-path=/usr/local/nginx/scgi_temp \
--user=nginx \
--group=nginx \
--with-mail \
--with-stream \
--with-threads \
--with-file-aio \
--with-poll_module \
--with-select_module \
--with-http_v2_module \
--with-http_flv_module \
--with-http_mp4_module \
--with-http_sub_module \
--with-http_dav_module \
--with-http_flv_module \
--with-http_ssl_module \
--with-http_geoip_module \
--with-http_slice_module \
--with-http_gunzip_module \
--with-http_realip_module \
--with-http_addition_module \
--with-http_image_filter_module \
--with-http_gzip_static_module \
--with-http_random_index_module \
--with-http_secure_link_module \
--with-http_degradation_module \
--with-http_stub_status_module \
--with-mail_ssl_module \
--with-stream_ssl_module \
--with-stream_realip_module \
--with-stream_ssl_preread_module \
--with-pcre=/usr/local/nginx/src/pcre-8.44 \
--with-openssl=/usr/local/nginx/src/openssl-1.1.1f \
--with-zlib=/usr/local/nginx/src/zlib-1.2.11
```
## 下载|安装
##### 下载压缩包
```bash

```
##### 解压压缩包
```bash
tar xf nginx1.18-offline-install.tar.gz
cd nginx1.18-offline-install
```
##### 执行安装脚本
```bash
source offline_install.sh
```
