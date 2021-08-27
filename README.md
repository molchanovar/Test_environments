# Test_environments
Test_labs 

## 1. Nginx front-end to apache web
 - Apache back-end and starts cgi-scripts

nginx.conf
```
    server {
        listen       80;
        listen       [::]:80;
        server_name  _;
        root         /usr/share/nginx/html;

        # Load configuration files for the default server block.
        include /etc/nginx/default.d/*.conf;

        location / {
                 proxy_pass http://10.83.79.123:80;
        }

```
