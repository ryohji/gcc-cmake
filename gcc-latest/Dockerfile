FROM gcc:7

RUN apt-get update && apt-get install -y --no-install-recommends \
    cmake \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

ADD protoc-3.5.1-linux-x86_64 /usr
