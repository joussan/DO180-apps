FROM ubi7/ubi:7.8
MAINTAINER "HASAN JOUAN"
LABEL description="A custom httpd container"
RUN yum update -y && yum install httpd -y && yum clean all
RUN echo "Hello from Dockerfile" > /usr/share/httpd/noindex/index.html
EXPOSE 80
ENTRYPOINT ["httpd", "-D", "FOREGROUND"]
