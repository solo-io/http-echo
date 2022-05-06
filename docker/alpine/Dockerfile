FROM alpine
ARG ARCH

ADD "https://curl.haxx.se/ca/cacert.pem" "/etc/ssl/certs/ca-certificates.crt"
ADD "./pkg/linux_${ARCH}/http-echo" "/"
RUN apk add curl
ENTRYPOINT ["/http-echo"]
