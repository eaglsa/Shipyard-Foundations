# Use the lightweight Nginx Alpine image as the base
FROM nginx:alpine

# Remove the default Nginx static assets to keep it clean
RUN rm -rf /usr/share/nginx/html/*

# Copy your custom index.html into the Nginx default public directory
# The path /usr/share/nginx/html/ is where Nginx looks for files by default
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80 (standard HTTP port)
EXPOSE 80

# The default command for the nginx image will automatically start the server