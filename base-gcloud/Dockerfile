FROM atox120/base:latest
MAINTAINER Alexander To <alexander.to@berkeley.edu> 

ENV SHELL /bin/bash

ENV DEBIAN_FRONTEND=non-interactive
ENV LC_ALL=C
ENV LANG=en_US.UTF-8
ENV LC_CTYPE=en_US.UTF-8

RUN echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
RUN apt-get install -y apt-transport-https ca-certificates gnupg
RUN curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key --keyring /usr/share/keyrings/cloud.google.gpg add -
RUN apt-get update && apt-get install -y google-cloud-sdk \
  google-cloud-sdk-app-engine-java \
  google-cloud-sdk-app-engine-python \
  google-cloud-sdk-app-engine-python-extras

WORKDIR $HOME
