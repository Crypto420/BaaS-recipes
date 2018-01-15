
# Copyright (c) 2017-2018 Morpheus Labs PTE LTD.

FROM eclipse/node

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN apk add -t .gyp --no-cache git python g++ make \
    && npm install -g truffle@3.2.x \
    && apk del .gyp

ENTRYPOINT ["truffle"]
