FROM centos:7
RUN yum install epel-release -y
RUN yum install nginx -y
RUN rm -rf /user/share/nginx/html/*
RUN echo "Hello World" > /user/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
LABEL COMPONENT=nginx