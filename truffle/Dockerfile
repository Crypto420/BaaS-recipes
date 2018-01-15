
# Copyright (c) 2017-2018 Morpheus Labs PTE LTD.

FROM eclipse/node

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# update the repository sources list
# and install dependencies
RUN apt-get update \
    && apt-get install -y curl git python build-essential \
    && npm install -g truffle@3.2.x \
    && apt-get -y autoclean
    
ENTRYPOINT ["truffle"]
