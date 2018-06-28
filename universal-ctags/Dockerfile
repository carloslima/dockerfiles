FROM debian:9.4-slim AS build

RUN apt-get update \
 && apt-get install --no-install-recommends -y make gcc autoconf git pkg-config automake libc6-dev ca-cacert
RUN git clone --depth=1 https://github.com/universal-ctags/ctags /ctags
RUN cd /ctags && ./autogen.sh && mkdir -p /opt/ctags && ./configure --prefix=/opt/ctags && make && make install

FROM debian:9.4-slim
COPY --from=0 /opt/ctags /opt/ctags
ENTRYPOINT /opt/ctags/bin/ctags
CMD "--help"
