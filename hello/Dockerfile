FROM golang:alpine as builder

RUN mkdir /build

ADD . /build

WORKDIR /build
RUN GOOS=linux GOARCH=amd64 go build -o hello main.go

FROM alpine
EXPOSE 8080

COPY --from=builder /build/hello /hello
ENTRYPOINT ["/hello"]
