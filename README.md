nginx.conf on masui.sfc.keio.ac.jp
==================================

copy to /usr/local/etc/nginx


build
-----

download nginx 1.3.16

- http://nginx.org/en/download.html


```
./configure \
--prefix=/usr/local \
--http-client-body-temp-path=/usr/local/tmp/nginx/client \
--http-proxy-temp-path=/usr/local/tmp/nginx/proxy \
--http-fastcgi-temp-path=/usr/local/tmp/nginx/fastcgi \
--conf-path=/usr/local/etc/nginx/nginx.conf \
--pid-path=/usr/local/var/run/nginx.pid \
--http-log-path=/usr/local/var/log/nginx/access.log \
--error-log-path=/usr/local/var/log/nginx/error.log \
--with-http_dav_module \
--with-http_mp4_module \
--with-http_secure_link_module \
--with-http_ssl_module \
--with-http_gzip_static_module \
--with-http_realip_module \
--with-http_stub_status_module \
--with-http_sub_module \
--with-http_xslt_module \
--with-mail \
--with-mail_ssl_module \
--without-http_uwsgi_module \
--without-http_scgi_module
```


ref
---

* https://gist.github.com/geta6/5380833
* http://shokai.org/blog/archives/7396
