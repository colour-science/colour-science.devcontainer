FROM ubuntu:jammy

ENV LANG C.UTF-8
ENV TZ=Etc/UTC

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update \
    && apt-get -y install software-properties-common \
    && add-apt-repository -y --update ppa:ansible/ansible \
    && apt-get -y install ansible \
    && apt-get autoremove -y \
    && apt-get clean -y
