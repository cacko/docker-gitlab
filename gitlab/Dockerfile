FROM yrzr/gitlab-ce-arm64v8
RUN mkdir -p /etc/gitlab
RUN mkdir -p /var/log/gitlab
RUN mkdir -p /var/opt/gitlab
RUN mkdir -p /assets
RUN chmod 777 /var/opt/gitlab
RUN /assets/update-permissions
RUN apt update
RUN apt install -y vim iproute2 
# RUN sed -in '/if \[ -n "${GITLAB_POST_RECONFIGURE_SCRIPT+x}" ]; then/ i exec /assets\/update-permissions' /assets/wrapper