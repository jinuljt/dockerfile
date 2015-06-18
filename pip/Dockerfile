FROM jinuljt/ubuntu:trusty

MAINTAINER juntao liu <jinuljt@gmail.com>

LABEL version="1.0"
LABEL description="pip 使用国内镜像"

# 安装pip
RUN apt-get update && apt-get install -y python-pip

# 指定pip使用国内镜像
RUN mkdir ~/.pip
COPY pip.conf ~/.pip/
