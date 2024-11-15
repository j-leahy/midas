FROM ubuntu:noble

ENV DEBIAN_FRONTEND=noninteractive

#Install tools
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git-all \
    && rm -rf /var/lib/apt/lists/*

#Launch shell
CMD ["/bin/bash"]