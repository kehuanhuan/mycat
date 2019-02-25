FROM java:8-jre
MAINTAINER <khh 1152018701@qq.com>
RUN wget http://dl.mycat.io/1.6-RELEASE/Mycat-server-1.6-RELEASE-20161028204710-linux.tar.gz
ENV mycat-version Mycat-server-1.6-RELEASE-20161028204710-linux.tar.gz
USER root
RUN tar -zxf /Mycat-server-1.6-RELEASE-20161028204710-linux.tar.gz
ENV MYCAT_HOME=/mycat
ENV PATH=$PATH:$MYCAT_HOME/bin
WORKDIR $MYCAT_HOME/bin
RUN chmod u+x ./mycat
EXPOSE 8066 9066
CMD ["./mycat","console"]