FROM node:10.16
MAINTAINER James Byars <jbyars4ku@gmail.com>

RUN apt-get update -y && apt-get install -y vim

WORKDIR /home

RUN npm install -g @angular/cli@8.2.0

EXPOSE 4200
