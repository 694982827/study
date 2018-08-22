### nginx 错误页面重定向





* 在nginx.conf配置页面需要开启`http{}`添加

  ```shell
  proxy_intercept_errors on;
  error_page  404 402 500 502 503 504  /50x.html;
    location = /50x.html {
              root   html;
              #root /var/www/html
            }	
  
  ```

  ​											