# Start from official Parrot Security base image
FROM parrotsec/security:latest

# Avoid user prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Update repos and install essentials
RUN apt update && \
    apt install -y \
        git \
        python3 \
        python3-pip \
        curl \
        wget \
        vim \
        net-tools \
        iputils-ping \
        dnsutils \
        nmap \
        gobuster \
        sqlmap \
        hydra \
        john \
        wfuzz \
        && apt clean && rm -rf /var/lib/apt/lists/*

# Set default shell
CMD ["/bin/bash"]
