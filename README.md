** proxy server example ** << Last Update : 2024.05.07 >>
 ┗ nginx-proxy
 ┗ tomcat-web
 ┗ nginx-alpine
   - os : alpine, x-forwarded-for off mode
   - $ docker build -t melca/nginx-alpine-proxy:1.0 .
   - $ docker run -itd -p 30080:80 --name nginx-alpine-proxy melca/nginx-alpine-proxy:1.0
 ┗ nginx-alpine-xff
   - os : alpine, x-forwarded-for on mode
   - $ docker build -t melca/nginx-alpine-proxy-xff:1.0 .
   - $ docker run -itd -p 30081:80 --name nginx-alpine-proxy-xff melca/nginx-alpine-proxy-xff:1.0
