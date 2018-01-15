
# Copyright (c) 2017-2018 Morpheus Labs PTE LTD.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html
# Contributors:
# Morpheus Labs PTE LTD. - truffle stack

FROM eclipse/node

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN apk add -t .gyp --no-cache git python g++ make \
    && npm install -g truffle@3.2.x \
    && apk del .gyp

ENTRYPOINT ["truffle"]
