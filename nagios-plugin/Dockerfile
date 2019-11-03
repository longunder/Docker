FROM centos:7
MAINTAINER longunder
RUN yum update -y && \
    yum install -y \
    wget \
    gcc \
    make && \
    yum clean all
RUN cd /usr/local/src/ && \
    wget https://nagios-plugins.org/download/nagios-plugins-2.2.1.tar.gz && \
    tar xzvf nagios-plugins-2.2.1.tar.gz && \
    cd /usr/local/src/nagios-plugins-2.2.1 && \
    ./configure && \
    make && \
    make install
