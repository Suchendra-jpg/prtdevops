# Use an official Ubuntu as a parent image
FROM ubuntu:latest

# Install Apache web server
RUN apt-get update -y && apt-get install -y apache2

# Copy your custom index.html into the default web server directory
COPY index.html /var/www/html/

# Expose port 80 to allow external access
EXPOSE 80

# Start Apache web server in the foreground
CMD ["apachectl", "-D", "FOREGROUND"]
