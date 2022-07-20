FROM yrzr/gitlab-ce-arm64v8
RUN mkdir -p /etc/gitlab
RUN mkdir -p /var/log/gitlab
RUN mkdir -p /var/opt/gitlab
RUN chmod 777 /var/opt/gitlab
RUN update-permissions
RUN apt update
RUN apt install -y vim iproute2 
COPY ./mente.sh /usr/sbin/mente.sh
RUN chmod +x /usr/sbin/mente.sh
CMD [ "/usr/sbin/mente.sh", "/usr/local/bin/wrapper" ]
