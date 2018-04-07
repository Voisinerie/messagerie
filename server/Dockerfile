FROM golang:1.10.1-alpine

WORKDIR /go/src/github.com/Voisinerie/messagerie/app
COPY ./app/ ./

RUN apk add --no-cache --update git
RUN go get github.com/pilu/fresh
RUN go get ./
RUN go build

EXPOSE 4000

CMD ["fresh"]
