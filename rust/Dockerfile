#
# Copyright 2022 Collabora, Ltd.
#
# SPDX-License-Identifier: MIT
#
FROM ghcr.io/atari-vcs/vcs-build-container:base
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    libssl-dev \
    ca-certificates \
    curl \
    pkg-config \
    build-essential

ARG RUSTUP_HOME=/opt/rust
ARG CARGO_HOME=/opt/rust
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --no-modify-path

ENV RUSTUP_HOME=/opt/rust
ENV CARGO_HOME=/opt/rust
ENV PATH="/opt/rust/bin:${PATH}"
