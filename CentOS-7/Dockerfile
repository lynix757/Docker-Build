FROM centos:7

RUN yum -y update && yum clean all
# Install EPEL Repo
RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm \
 && rpm -Uvh http://rpms.remirepo.net/enterprise/remi-release-7.rpm

ENV TIMEZONE Asia/Bangkok
RUN cp /usr/share/zoneinfo/${TIMEZONE} /etc/localtime \
&& echo "${TIMEZONE}" >  /etc/timezone

RUN yum -y update
RUN yum -y install ntp \
                   net-tools \
                   traceroute \
                   bind-utils \
                   vim \
    yum clean all && \
    rm -rf /var/cache/yum
