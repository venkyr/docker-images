# Use the official BusyBox base image
FROM busybox:latest

# Install curl binary (pre-compiled)
RUN wget --no-check-certificate https://github.com/stunnel/static-curl/releases/download/8.4.0/curl-static-amd64-8.4.0.tar.xz -O /tmp/curl.tar.xz \
    && cd /tmp \
    && tar -xzJf curl.tar.xz \
    && cp /tmp/curl /bin/curl \
    && chmod +x /bin/curl

RUN rm -rf /tmp/*

CMD ["/bin/sh"]
