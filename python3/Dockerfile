FROM ubuntu:latest

MAINTAINER juntao liu <jinuljt@gmail.com>

LABEL version="1.0"
LABEL description="based on ubuntu:xenial\n\
aliyun apt source mirror\n\
\n\
include python3/pip3/supervisor\n\
\n\
supervisord.conf \n\
minfds=102400\n\
minprocs=102400\n"


# 换apt mirror
COPY sources.list /etc/apt/sources.list


# 安装pip
RUN apt-get update &&  apt-get install -y \
    python3 \
    python3-pip \
    supervisor \
&& rm -rf /var/lib/apt/lists/*
