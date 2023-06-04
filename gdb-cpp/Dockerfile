FROM  ubuntu:bionic

LABEL maintainer="Pradeep Suthar <pradeexsu@gmail.com>"
# Git repo: https://github.com/pradeexsu/docker-images.git

# Install necessary dependencies
RUN apt-get update &&\
    apt-get install -y --no-install-recommends \
    g++ \
    build-essential \
    autoconf \
    automake \
    libtool \
    pkg-config \
    apt-transport-https \
    ca-certificates \
    software-properties-common \
    wget \
    git \
    curl \
    gnupg \
    zlib1g-dev \
    swig \
    vim \
    gdb \
    valgrind \
    locales \
    locales-all &&\
    apt-get clean


# setting up .vimrc
RUN echo "syntax on\n\
    set nu\n\
    set rnu\n\
    set ts=4\n\
    set ai\n\
    set sw=4\n\
    set ss=4\n\
    set smarttab\n\
    set expandtab\n\
    set smartcase\n\
    set tags=tags\n\
    set t_Co=256\n\
    set encoding=utf-8\n\
    let g:airline_powerline_fonts = 1" > ~/.vimrc

ENV LC_ALL en_US.UTF-8
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US.UTF-8

