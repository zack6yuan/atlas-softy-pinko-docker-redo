# Latest version of nginx
FROM nginx:latest
# Copy files.
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end
# Create Nginx config.
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
# Expose the correct port
EXPOSE 9000