
# Copyright (c) 2017-2018 Morpheus Labs PTE LTD.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html

# Contributors:
# Morpheus Labs PTE LTD.
FROM node:7.4-alpine

RUN apk add -t .gyp --no-cache git python g++ make \
    && npm install -g ethereumjs-testrpc@3.0.x \
    && apk del .gyp
RUN apk add --update bash && rm -rf /var/cache/apk/*
EXPOSE 8545
ENTRYPOINT ["testrpc"]
