FROM ubuntu:18.04

RUN apt-get update \
    && apt-get install -y git \
    && apt-get install -y python3 \
    && apt-get install -y python3-pip \
    && apt-get install -y emacs

RUN pip3 install flask \
    && pip3 install --upgrade flask \
    && pip3 install mysql-connector-python

ENV APP_PATH=/home
WORKDIR $APP_PATH
ENV HOME $APP_PATH

CMD [ "/bin/sh" ]