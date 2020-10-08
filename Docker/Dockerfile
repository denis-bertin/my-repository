docker build -t ansible-juniper-junos:latest -f- . <<EOF
FROM alpine
RUN apk update
RUN apk upgrade
RUN apk add ansible
RUN ansible-galaxy install juniper.junos
RUN apk update
RUN mkdir /etc/ansible
RUN mkdir /etc/ansible
RUN touch /etc/ansible/hosts
VOLUME /Utilisateur
EOF