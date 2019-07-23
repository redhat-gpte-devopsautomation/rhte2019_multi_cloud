FROM fedora:30

RUN cd /tmp \
  && dnf -y update \
  && dnf install -y skopeo

ADD script.sh /usr/local/bin/skopeo

ENTRYPOINT ["/usr/local/bin/skopeo"]

CMD ["help"]