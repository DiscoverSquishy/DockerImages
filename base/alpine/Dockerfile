FROM alpine:3.20

LABEL os="Alpine" author="DiscoverSquishy" maintainer="noaimi2214@gmail.com"
RUN adduser -D -h /home/container container && \
    apk --no-cache add \
        ca-certificates \
        curl \
        openssl \
        git \
        tar \
        jq \
        tzdata \
        sqlite \
        fontconfig \
        iproute2 \
        freetype \
        python3 \
    && rm -rf /var/cache/apk/*

# Package cleanup
RUN rm -rf /var/cache/apk/*