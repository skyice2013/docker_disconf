FROM maven:3.5.3-jdk-8
MAINTAINER qilong <qilong628@163.com>

RUN curl -fSL https://github.com/knightliao/disconf/archive/2.6.36.zip -o 2.6.36.zip
RUN unzip 2.6.36.zip
ENV ONLINE_CONFIG_PATH /home/work/dsp/disconf-rd/online-resources
ENV WAR_ROOT_PATH /home/work/dsp/disconf-rd/working/war
RUN cd disconf-2.6.36/disconf-web
VOLUME /home/work/dsp/disconf-rd/online-resources
VOLUME /home/work/dsp/disconf-rd/working
WORKDIR disconf-2.6.36/disconf-web
CMD ["sh", "deploy/deploy.sh"]