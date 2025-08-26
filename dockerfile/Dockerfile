# Use the official Nginx image as base
FROM nginx:alpine

# Remove the default Nginx welcome page
RUN rm /usr/share/nginx/html/index.html

# Copy your custom index.html file
COPY index.html /usr/share/nginx/html/

# Expose port 80 (Nginx default port)
EXPOSE 80

# Command to run Nginx (inherited from base image)
CMD ["nginx", "-g", "daemon off;"]