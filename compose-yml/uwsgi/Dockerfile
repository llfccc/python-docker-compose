# base image
FROM python:3.5.4

# MAINTAINER
MAINTAINER lelinfeng

#3.复制requirements.txt
ADD ./back_uwsgi.ini /opt/server/ 
ADD ./requirements.txt /opt/temp/ 
#RUN pip install -r /opt/temp/requirements.txt -i  https://pypi.douban.com/simple/ 

RUN mkdir -p /opt/temp/
RUN mkdir -p /opt/server 
WORKDIR /opt/server

#ADD ./LiuFuYa /opt/server/LiuFuYa
 
CMD ['cat','/opt/server/back_uwsgi.ini']

EXPOSE 8000
