FROM ubuntu:16.04

RUN apt-get update
RUN apt-get install -y htop gcc build-essential libncurses-dev bison flex libssl-dev libelf-dev
RUN apt-get install -y bc kmod
RUN apt-get install -y apt-utils initramfs-tools

ENTRYPOINT /bin/bash

