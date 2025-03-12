FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y iputils-ping && \
    apt-get install -y iproute2 && \
    apt-get install -y netcat && \
    apt-get install -y curl && \
    apt-get install -y apache2 && \
    apt-get install -y strongswan && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]