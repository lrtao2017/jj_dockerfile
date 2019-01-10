# yum install nginx 
# 20190109

FROM centos7.5:yum

MAINTAINER lrtao2010@163.com


#添加yum源
COPY nginx.repo /etc/yum.repos.d/
RUN yum install nginx -y
COPY nginx.conf /etc/nginx/
RUN rm -rf /etc/nginx/conf.d/default.conf

#启动nginx
CMD /usr/sbin/nginx -c /etc/nginx/nginx.conf
