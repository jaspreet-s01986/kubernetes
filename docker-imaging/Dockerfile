FROM centos:7
RUN yum install epel-release -y
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/*
# RUN echo "Hello World" > /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/index.html
# EXPOSE doens't make any difference but is just for representational & human readable format only
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
# LABEL COMPONENT=nginx
# ENV variables can also be used.
ENV COMPONENT=nginx
LABEL COMPONENT=${COMPONENT}