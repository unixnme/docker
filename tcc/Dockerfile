FROM ubuntu:18.04

WORKDIR /usr/src/tcc

RUN apt-get update && apt-get install -y build-essential wget vim

RUN wget http://download.savannah.gnu.org/releases/tinycc/tcc-0.9.27.tar.bz2 && tar jxf tcc-0.9.27.tar.bz2

RUN cd tcc-0.9.27 && ./configure && make -j `nproc` && make install

