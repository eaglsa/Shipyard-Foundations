FROM nginx:alpine

# 1. Clean out the default Nginx directory
RUN rm -rf /usr/share/nginx/html/*

# 2. Copy your index.html as a template
# Nginx will look here, swap the variables, and put it in /usr/share/nginx/html/
COPY index.html /etc/nginx/templates/index.html.template

# 3. Ensure permissions are wide open so Nginx can read it
RUN chmod 644 /etc/nginx/templates/index.html.template

EXPOSE 80