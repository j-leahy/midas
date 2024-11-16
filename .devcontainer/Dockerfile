FROM ubuntu:noble

ENV DEBIAN_FRONTEND=noninteractive

#Install tools
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git-all \
    && rm -rf /var/lib/apt/lists/*

#Install Rust
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
ENV PATH="/root/.cargo/bin:${PATH}"

#Launch shell
CMD ["/bin/bash"]