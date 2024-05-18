FROM nginx:alpine
RUN apk --update --no-cache add curl
EXPOSE 80
COPY ./configuration/nginx.conf /etc/nginx/nginx.conf
RUN rm -rf /usr/share/nginx/html/*
COPY /pages /usr/share/nginx/html
ENTRYPOINT ["nginx", "-g", "daemon off;"]
RUN rm -rf /var/cache/apk/*
