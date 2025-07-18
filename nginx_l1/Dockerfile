FROM nginx:alpine
# Remove default Nginx config to ensure yours is used
RUN mkdir -p /var/cache/nginx && chown -R nginx:nginx /var/cache/nginx
RUN rm /etc/nginx/conf.d/default.conf
# Copy custom Nginx configuration
COPY nginx.conf /etc/nginx/conf.d/default.conf
# ... other configurations like mkdir and chown ...
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]