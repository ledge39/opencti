FROM certbot/certbot:latest

# Install git and pip dependencies using Alpine package manager
RUN apk add --no-cache git py3-pip

# Copy the plugin code into the container
COPY certbot_dns_ionos-master /opt/certbot-dns-ionos

# Move into the plugin directory and install it
WORKDIR /opt/certbot-dns-ionos
RUN pip install .
