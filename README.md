# Test_environments
Test_labs 

## 1. Nginx front-end to apache web
 - Apache as a back-end and runs cgi-scripts

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
