# http-code-test-nginx-config
Routes with standard http responses for testing response handling


```
server {    
    
    # ...

    add_header X-Frame-Options "SAMEORIGIN";
    add_header X-XSS-Protection "1; mode=block";
    add_header X-Content-Type-Options "nosniff";
    add_header Content-Type text/plain;

    #location /100 { return 100 'Continue';}
    #location /101 { return 101 'Switching Protocols';}
    location /200 { return 200;}
    location /201 { return 201;}
    location /202 { return 202;}
    location /203 { return 203;}
    location /204 { return 204;}
    location /205 { return 205;}
    location /206 { return 206;}
    location /300 { return 300;}
    location /301 { return 301;}
    location /302 { return 302;}
    location /303 { return 303;}
    location /305 { return 305;}
    location /307 { return 307;}
    location /400 { return 400;}
    location /401 { return 401;}
    location /402 { return 402;}
    location /403 { return 403;}
    location /404 { return 404;}
    location /405 { return 405;}
    location /406 { return 406;}
    location /407 { return 407;}
    location /408 { return 408;}
    location /409 { return 409;}
    location /410 { return 410;}
    location /411 { return 411;}
    location /412 { return 412;}
    location /413 { return 413;}
    location /414 { return 414;}
    location /415 { return 415;}
    location /416 { return 416;}
    location /417 { return 417;}
    location /418 { return 418;}
    location /429 { return 429;}
    location /431 { return 431;}
    location /451 { return 451;}
    location /500 { return 500;}
    location /501 { return 501;}
    location /502 { return 502;}
    location /503 { return 503;}
    location /504 { return 504;}
    location /505 { return 505;}
    location /511 { return 511;}

    location = /favicon.ico { access_log off; log_not_found off; }
    location = /robots.txt  { access_log off; log_not_found off; }

    access_log off;

    location / {
        return 200;
    }

}
```
