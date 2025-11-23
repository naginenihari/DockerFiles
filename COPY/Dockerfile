FROM nginx
RUN rm -rf /usr/share/nginx/html/index.html
#COPY index.html /usr/share/nginx/html/index.html
COPY qi/ /usr/share/nginx/html/
CMD ["nginx","-g","daemon off;"]


## COPY is used to copy the files and directories from local to image.
## The index.html file is current directory should be copy where the dockerfile