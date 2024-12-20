FROM ubuntu:latest
RUN apt-get -y update &&  apt-get install -y nginx && apt-get install -y curl
COPY nginx.conf /etc/nginx/conf.d/default.conf
COPY index.html /usr/share/nginx/html/index.html 
# RUN sed -i 's/listen 80;/listen 8080;/' /etc/nginx/sites-available/default
EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]