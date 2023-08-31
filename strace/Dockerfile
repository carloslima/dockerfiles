FROM ubuntu:23.04 AS build

RUN apt-get update
RUN apt-get install -y build-essential autoconf git

RUN git clone https://github.com/strace/strace /code
WORKDIR /code

RUN ./bootstrap
RUN ./configure --disable-mpers LDFLAGS='-static -pthread'
RUN make
RUN ./src/strace -h

FROM ubuntu:23.04 AS runtime
COPY --from=build /code/src/strace /bin/strace
