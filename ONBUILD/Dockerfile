FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ONBUILD COPY index.html /usr/share/nginx/html/index.html
CMD ["nginx","-g","daemon off;"]



## ONBUILD will instruct users to follow rules while building. while building this image onbuild will not run. If someone uses our image i will instruct the user to maintian index.html in there folder.