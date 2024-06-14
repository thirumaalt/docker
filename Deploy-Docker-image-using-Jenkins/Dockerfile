# Use the official Nginx image as the base image
FROM nginx:latest

# Copy the HTML, CSS, and JS files into the Nginx document root directory
COPY index.html /usr/share/nginx/html/
COPY styles.css /usr/share/nginx/html/
COPY script.js /usr/share/nginx/html/

# Expose port 80 to allow external access
EXPOSE 80
