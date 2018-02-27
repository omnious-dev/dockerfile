#
# filebeat-log-forwarder
#
# build:
#   docker build --force-rm -t omniousdev/filebeat-log-forwarder .
# run:
#   docker run \
#     --rm --it \
#     --network host \
#     --volume /var/run/docker.sock:/var/run/docker.sock \
#     --volume filebeat-data:/usr/share/filebeat/data \
#     --volume app-log:/log \
#     --name filebeat-log-forwarder \
#     omniousdev/filebeat-log-forwarder
#

FROM docker.elastic.co/beats/filebeat:6.2.0
LABEL maintainer "Omnious Dev <dev@omnious.com>"

# Copy configurations
COPY filebeat.yml /usr/share/filebeat/filebeat.yml
# Update file permission
USER root
