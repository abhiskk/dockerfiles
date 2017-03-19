FROM darkstar112358/dl-py3
MAINTAINER Abhishek Kadian <abhishekkadiyan@gmail.com>

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update -qy

RUN pip3 install cmake
RUN pip3 install numpy --upgrade
RUN pip3 install scipy --upgrade
RUN pip3 install git+https://github.com/pytorch/pytorch.git@master --upgrade
RUN pip3 install torchvision
