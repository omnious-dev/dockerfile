#
# docker-cd
#
# build:
#   docker build --force-rm -t omniousdev/docker-cd .
# run:
#   docker run --rm --name docker-cd omniousdev/docker-cd
#

FROM docker:18.01.0-ce
LABEL maintainer "Omnious Dev <dev@omnious.com>"

# Install needed packages
RUN apk --no-cache add python py-pip git openssh-client

RUN pip install awscli
