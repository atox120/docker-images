FROM ubuntu:focal
MAINTAINER Alexander To <alexander.to@berkeley.edu> 
## Based off original image from Mark Mims Mark Mims <mark.mims@gmail.com>

ENV SHELL /bin/bash
ENV NB_USER science
ENV NB_UID 1000
ENV HOME /base

ENV DEBIAN_FRONTEND=non-interactive
ENV LC_ALL=C
ENV LANG=en_US.UTF-8
ENV LC_CTYPE=en_US.UTF-8

## expose ports for jupyter notebook
EXPOSE 8888

VOLUME /base

COPY policy-rc.d /usr/sbin
COPY scripts/* /tmp/

RUN bash /tmp/010-packages
RUN bash /tmp/050-1click-base
RUN bash /tmp/051-1click-python
## RUN bash /tmp/071-gcloud-sdk

WORKDIR $HOME
