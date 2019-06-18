FROM python:3.6-alpine

RUN pip install --no-cache-dir rdbtools==0.1.14
RUN apk add --no-cache --virtual .build-deps gcc musl-dev && \
    pip install --no-cache-dir python-lzf==0.2.4 && \
    apk del .build-deps gcc musl-dev
WORKDIR /data

ENTRYPOINT ["rdb"]
