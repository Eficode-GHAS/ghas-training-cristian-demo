FROM debian:stable-slim

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get -yq update && apt-get -yq upgrade
RUN apt-get -yq install unzip git curl apt-transport-https build-essential sudo

RUN curl -sL https://golang.org/dl/go1.15.3.linux-amd64.tar.gz --output go1.15.3.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf go1.15.3.linux-amd64.tar.gz
RUN curl -sL https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb --output packages-microsoft-prod.deb
