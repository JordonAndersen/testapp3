FROM nginx:alpine

COPY index.html pkbld.html loginstyle.css style.css app.js   /usr/share/nginx/html/
COPY images/ /usr/share/nginx/html/images/
COPY ./*.html ./*.css ./*.js ./**/*.jpg ./**/*.png /usr/share/nginx/html/