FROM nginx:alpine
EXPOSE 80
COPY ./configuration/nginx.conf /etc/nginx/nginx.conf
RUN rm -rf /usr/share/nginx/html/*
COPY /pages /usr/share/nginx/html
ENTRYPOINT ["nginx", "-g", "daemon off;"]
