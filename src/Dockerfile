ARG FROM_TAG

FROM debian:${FROM_TAG:-bullseye}

RUN apt-get update -y && \
    apt-get install -y rsync && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["rsync"]
