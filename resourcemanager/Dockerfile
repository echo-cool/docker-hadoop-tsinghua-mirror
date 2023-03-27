FROM bde2020/hadoop-base:2.0.0-hadoop3.2.1-java8

MAINTAINER Ivan Ermilov <ivan.s.ermilov@gmail.com>

HEALTHCHECK CMD curl -f http://localhost:8088/ || exit 1

<<<<<<< HEAD

RUN echo "" > /etc/apt/sources.list
RUN echo "deb http://mirrors.tuna.tsinghua.edu.cn/debian/ stretch main contrib non-free" >> /etc/apt/sources.list
RUN echo "deb http://mirrors.tuna.tsinghua.edu.cn/debian/ stretch-updates main contrib non-free" >> /etc/apt/sources.list
RUN echo "deb http://mirrors.tuna.tsinghua.edu.cn/debian/ stretch-backports main contrib non-free" >> /etc/apt/sources.list
RUN echo "deb http://mirrors.tuna.tsinghua.edu.cn/debian-security stretch/updates main contrib non-free" >> /etc/apt/sources.list
RUN apt update && apt install python3 -y

=======
>>>>>>> 8414e2b05122f85392cce0d27bf3978ed056696e
ADD run.sh /run.sh
RUN chmod a+x /run.sh

EXPOSE 8088

CMD ["/run.sh"]
