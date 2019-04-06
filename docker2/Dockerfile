# Version: 0.0.1
FROM fedora
MAINTAINER maintainer_name "maintainer_email"
RUN dnf update -y
RUN dnf install -y nginx net-tools procps htop atop
RUN echo 'Default page. Nginx is in your container. ' \
>/usr/share/nginx/html/index.html
EXPOSE 80
WORKDIR /srv
RUN mkdir -p /srv
CMD ["nginx", "-g", "daemon off;"]
#CMD ["/bin/sh", "-c", "nginx > server.log 2>&1"]
