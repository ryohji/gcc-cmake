FROM gcc:7

RUN apt-get update && apt-get install -y --no-install-recommends \
    cmake \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

ADD protobuf-cpp-3.5.1.tar.gz /tmp
RUN cd /tmp/protobuf-3.5.1 && ./autogen.sh\
 && ./configure --prefix=/usr --disable-shared\
 && make install && ldconfig\
 && rm -r /tmp/protobuf-3.5.1
