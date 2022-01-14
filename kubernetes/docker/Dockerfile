FROM golang:1.13.8-alpine3.11 as golang1
WORKDIR src
COPY src/hello.go .
RUN CGO_ENABLED=0 go build -ldflags="-s -w" -o /hello

FROM scratch
COPY --from=golang1 /hello /hello
ENTRYPOINT ["/hello"]
