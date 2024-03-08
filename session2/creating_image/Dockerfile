FROM centos:7

LABEL author="Pavel"

LABEL Remarks="This is a dockerfile example for CentOS system"

RUN yum -y update && yum -y install httpd && yum clean all

EXPOSE 80

WORKDIR /root