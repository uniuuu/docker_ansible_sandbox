# Version: 0.0.1
FROM debian
MAINTAINER maintainer_name "maintainer_email"
RUN apt update
RUN apt install -y nginx net-tools procps htop atop curl
RUN echo 'Default page. Nginx is in your container. ' \
>/var/www/html/index.html
#WORKDIR /etc/nginx/
#COPY append_conf_nginx ./
#RUN sed -i -e '0,/http\ {/{/http\ {/r append_conf_nginx' -e '}' nginx.conf
EXPOSE 80
RUN mkdir -p /srv
#VOLUME /root/docker_project /srv
CMD ["nginx", "-g", "daemon off;"]
