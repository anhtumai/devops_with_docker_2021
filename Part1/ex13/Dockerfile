FROM golang:1.16-buster

WORKDIR /usr/src/app

COPY /material-applications/example-backend /usr/src/app

EXPOSE 8080

RUN go build

ENTRYPOINT ["./server"]

