FROM nginx:latest

# Copy Nginx configuration file
COPY ./nginx_conf/nginx.conf /etc/nginx/nginx.conf

# Copy CDN resources
COPY ./cdn/ /usr/share/nginx/html
