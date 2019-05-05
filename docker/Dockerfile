FROM alpine

RUN groupadd kovend && useradd kovend
RUN apk add python

COPY koven /srv/
RUN ln /srv/koven/kovend /usr/local/bin/kovend

USER kovend:kovend

ENTRYPOINT ["/usr/local/bin/kovend"]
