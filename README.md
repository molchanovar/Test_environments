# Test_environments
Test_labs 

## 1. Nginx front-end to apache web
 - Apache back-end and starts cgi-scripts

nginx.conf
```
    server {
...
        location / {
                 proxy_pass http://10.83.79.123:80;
        }
...
}
```
