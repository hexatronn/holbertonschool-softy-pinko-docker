FROM docker.io/library/nginx:latest

# Copy frontend files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
