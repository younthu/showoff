# nginx configuration at /etc/nginx/sites-available

~~~
server {
  listen 80;
  server_name timage.ilibrary.me;
  root /home/deployer/wwwroot/showoff;
  location / {
        proxy_pass http://127.0.0.1:5050;
    }

}
~~~

# nginx 日志查看
cat /var/log/nginx/error.log
cat /etc/nginx/nginx.conf
