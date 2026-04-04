FROM nginx:latest

# Remove default config
RUN rm /etc/nginx/conf.d/default.conf

# Copy your custom config
COPY fdx-ui/default.conf /etc/nginx/conf.d/

# Copy static files (NOT WAR)
COPY fdx-ui/ /usr/share/nginx/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
