FROM nginx:latest
# set error logs to debug level
RUN sed -ie 's|error_log .*|error_log /var/log/nginx/error.log debug;|g' /etc/nginx/nginx.conf
# disable access logs
RUN sed -ie 's|access_log .*|access_log off;|g' /etc/nginx/nginx.conf

# Для более сложных изменений логирования можно
# COPY nginx.conf /etc/nginx/nginx.conf