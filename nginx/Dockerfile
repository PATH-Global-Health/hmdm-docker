FROM nginx:1.25-alpine
LABEL maintainer="Belendia Serda belendia@gmail.com"

ADD ./nginx/nginx.conf /etc/nginx/nginx.conf
RUN rm /etc/nginx/conf.d/default.conf
COPY ./volumes/work/files /usr/share/nginx/html/files
# COPY ./volumes/lib /usr/share/nginx/html/lib
EXPOSE 8888
CMD ["nginx", "-g", "daemon off;"]