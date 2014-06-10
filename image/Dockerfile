FROM ubuntu:12.04
MAINTAINER Danilo Bardusco <bardusco@gmail.com>

ENV HOME /root
RUN mkdir /build
ADD . /build

RUN /build/prepare.sh
RUN	/build/system_services.sh
RUN	/build/utilities.sh
RUN	/build/cleanup.sh

CMD ["/sbin/my_init"]
