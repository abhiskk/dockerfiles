FROM ubuntu:latest
MAINTAINER Abhishek Kadian <abhishekkadiyan@gmail.com>

ARG DEBIAN_FRONTEND=noninteractive
ENV PYTHONIOENCODING=utf8
RUN locale-gen en_US.UTF-8
ENV LC_ALL=en_US.UTF-8

RUN apt-get update -qy
RUN apt-get install -qy libopenblas-dev
RUN apt-get install -qy python3-pip
RUN apt-get install -qy python3-numpy
RUN apt-get install -qy python3-scipy
RUN apt-get install -qy python3-matplotlib
RUN apt-get install -qy dvipng
RUN apt-get install -qy git
RUN apt-get install -qy tmux
RUN apt-get install -qy htop

RUN pip3 install scikit-learn
RUN pip3 install seaborn
RUN pip3 install tqdm
RUN pip3 install ipython
RUN pip3 install jupyter

RUN mkdir -p /root/.jupyter/custom
RUN mkdir -p /root/.local/share/jupyter/nbextensions

EXPOSE 9999

RUN mkdir /root/.matplotlib

RUN apt-get install -qy vim
