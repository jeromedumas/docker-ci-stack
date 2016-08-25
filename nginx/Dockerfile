FROM nginx:1.10.1

MAINTAINER jerome.dumas

RUN rm /etc/nginx/conf.d/default.conf

COPY assets/etc/nginx/conf.d/jenkins.conf /etc/nginx/conf.d/jenkins.conf
COPY assets/etc/nginx/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80 
EXPOSE 443

CMD ["nginx"]
