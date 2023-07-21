FROM nginx:alpine

# Remove the default Nginx configuration
RUN rm -rf /etc/nginx/conf.d/*

# Copy the static files to the Nginx document root
COPY . /usr/share/nginx/html


EXPOSE 80

# Start the Nginx server
CMD ["nginx", "-g", "daemon off;"]