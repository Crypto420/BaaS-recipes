
# Copyright (c) 2017-2018 Morpheus Labs PTE LTD.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html

# Contributors:
# Morpheus Labs PTE LTD.
FROM eclipse/ubuntu_go

# update the repository sources list
# install docker and ependencies
RUN apt-get update \
  && apt-get install -y apt-transport-https ca-certificates curl software-properties-common \
  && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - \
  && add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
  && apt-get update \
  && apt-get install docker-ce -y
  && apt-get -y autoclean

# install docker composer
RUN curl -L https://github.com/docker/compose/releases/download/1.18.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
RUN chmod +x /usr/local/bin/docker-compose

CMD tail -f /dev/null
