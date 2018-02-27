# @edt ASIX M11 2017-2018
# ldapserver:datadb
# Servidor ldap creacio interactiva
# ----------------------------------
FROM fedora:24
MAINTAINER vladimir-remar@edt "ASIX M06/M11 @edt 2015-16"
RUN dnf update vi -y
RUN dnf -y install openldap openldap-servers openldap-clients iproute tree nmap vim procps iputils mlocate man-db
RUN mkdir /opt/docker
COPY * /opt/docker/
RUN /opt/docker/install.sh
WORKDIR /opt/docker
CMD ["/opt/docker/startup.sh"]
