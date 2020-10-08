FROM alpine:3.6
RUN apk update && apk add --no-cache \
    openssl \
    ca-certificates \
    python \
    py-pip \
    python-dev \
    libffi-dev \
    openssl-dev \
    build-base \
    git
RUN pip install ansible
RUN ansible-galaxy install Juniper.junos
WORKDIR /playbooks
VOLUME /playbooks
CMD [ "ansible", "--version" ]