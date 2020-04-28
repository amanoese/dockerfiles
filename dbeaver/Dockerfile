FROM openjdk:11

RUN wget -O - https://dbeaver.io/debs/dbeaver.gpg.key | apt-key add -
RUN echo "deb https://dbeaver.io/debs/dbeaver-ce /" | tee /etc/apt/sources.list.d/dbeaver.list

RUN apt-get update
RUN apt-get install dbeaver-ce -y

CMD dbeaver
