# Use the official lightweight Nginx image based on Alpine Linux
FROM nginx:alpine

# Copy website files
COPY index.html pkbld.html loginstyle.css style.css app.js /usr/share/nginx/html/
COPY images/ /usr/share/nginx/html/images/
COPY ./*.html ./*.css ./*.js ./**/*.jpg ./**/*.png /usr/share/nginx/html/

# Copy the Nginx configuration file
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Expose port 80 (adjust if needed)
EXPOSE 80

# Start the Nginx process in the foreground
CMD ["nginx", "-g", "daemon off;"]
