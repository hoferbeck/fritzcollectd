FROM alpine

# Install collectd and dependencies for fritzcollectd.
RUN apk add --no-cache \
        collectd \
        collectd-python \
        collectd-network \
        python3 \
        py-pip \
        py-lxml \
        py-pbr \
        git

# Copy entrypoint script.
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
