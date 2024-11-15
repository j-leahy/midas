FROM ubuntu:noble

ENV DEBIAN_FRONTEND=noninteractive

#Install tools
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git-all \
    python3 \
    python3-pip\
    && rm -rf /var/lib/apt/lists/*

#Rust install
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
ENV PATH="/root/.cargo/bin:${PATH}"

#Launch shell
CMD ["/bin/bash"]