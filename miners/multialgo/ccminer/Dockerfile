FROM perfectweb/base:cuda-9.0-devel-ubuntu16.04
MAINTAINER Alin Jurj <office@perfectweb.ro>

RUN git clone -b 2.2.5-tpruvot https://github.com/tpruvot/ccminer.git
RUN cd /ccminer && ./build.sh

ENTRYPOINT ["/ccminer/ccminer"]
CMD ["-a", "lbry", "-o", "stratum+tcp://lbry.suprnova.cc:6256", "-u", "Tahity.default", "-p", "x"]
