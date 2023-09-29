FROM golang:1-alpine

RUN apk add --no-cache git \
  && git clone https://github.com/heroes1412/dos-hulk-go.git \
  && cd /go/hulk \
  && go install \
  && rm -rf /go/hulk \
  && apk del git

ENTRYPOINT ["hulk"]

CMD ["--help"]
