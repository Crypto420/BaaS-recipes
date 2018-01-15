
# Copyright (c) 2012-2016 Codenvy, S.A.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html

# Contributors:
# Morpheus Labs PTE LTD.
FROM eclipse/node

USER root
# update the repository sources list
# and install dependencies
RUN apt-get update \
    && apt-get install -y curl git python build-essential \
    && npm install -g truffle@3.2.x \
    && apt-get -y autoclean
CMD tail -f /dev/null
