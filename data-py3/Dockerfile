FROM python:3.5

MAINTAINER Zhongwen Song <tjsongzw@gmail.com>

ENV PYTHONUNBUFFERED 1

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        libatlas-base-dev gfortran

RUN mkdir -p /opt/data-py3/build

COPY requirements.txt /opt/data-py3/build/requirements.txt

RUN pip install -r /opt/data-py3/build/requirements.txt