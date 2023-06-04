FROM  ubuntu:bionic

LABEL maintainer="Pradeep Suthar <pradeexsu@gmail.com>"

# Git repo: https://github.com/pradeexsu/docker-images.git

# installing  
RUN apt-get update && apt-get -y install g++ gdb vim

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

