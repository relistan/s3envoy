FROM alpine:latest

RUN apk add --no-cache ca-certificates
ADD s3proxy /s3proxy/
ADD config.json /s3proxy/
WORKDIR /s3proxy
CMD ["/s3proxy/s3proxy", "-config", "config.json"]
