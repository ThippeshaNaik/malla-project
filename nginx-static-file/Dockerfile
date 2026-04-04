FROM nginx:latest
RUN rm /etc/nginx/conf.d/default.conf
COPY fdx-ui/default.conf /etc/nginx/conf.d

RUN rm -rf /usr/share/nginx/html

COPY fdx-ui /usr/share/nginx/html

ENTRYPOINT ["nginx","-g","daemon off;"]

