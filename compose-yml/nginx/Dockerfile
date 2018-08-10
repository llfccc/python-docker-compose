# base image
FROM nginx:1.15.2

# MAINTAINER
MAINTAINER lelinfeng

#3.安装yum二外软件包
ADD ./nginx.conf /etc/nginx
ADD ./liufuya_nginx.conf /etc/nginx/conf.d/

VOLUME [ "/opt/code/client" ]
ADD ./run.sh  /

CMD ["/bin/bash","/run.sh"]    
EXPOSE 80
