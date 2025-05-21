# Creating the base image for the nginx server
FROM nginx:1.21.6-alpine 

# Removing the default nginx configuration file 
RUN rm -rf /etc/nginx/conf.d/default.conf

# Copying the nginx configuration file to the image
COPY nginx.conf /etc/nginx/conf.d/default.conf

