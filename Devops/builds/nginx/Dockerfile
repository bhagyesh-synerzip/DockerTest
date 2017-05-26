# This is the demonstration for an nginx server to copy and run directly from git
FROM nginx:latest

MAINTAINER bhagyesh.raut@synerzip.com

RUN apt-get update && apt-get install -y git

RUN mkdir /app

WORKDIR /app 

RUN git clone https://github.com/bhagyesh-synerzip/DockerTest.git

COPY ./DockerTest /usr/share/nginx/html

EXPOSE 80
