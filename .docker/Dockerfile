FROM ubuntu:16.04

RUN apt-get update && apt-get install -y --no-install-recommends \
    software-properties-common \
    && add-apt-repository -y  ppa:gophers/archive \
    && apt-get update && apt-get install -y \
        golang-1.10-go \
        vim \
        less \
        git-all \
        curl \
    && rm -rf /var/lib/apt/lists/*

ENV PATH "/usr/lib/go-1.10/bin/:$PATH" 

CMD ["/bin/bash"]
