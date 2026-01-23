FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && \
    apt install -y \
        git \
        openjdk-21-jdk \
        ca-certificates \
    && rm -rf /var/lib/apt/lists/*
