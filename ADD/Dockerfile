FROM almalinux:9 
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://stackoverflow.com/questions/30853247/how-do-i-edit-a-file-after-i-shell-to-a-docker-container /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]