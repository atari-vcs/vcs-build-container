#
# Copyright 2021 Collabora, Ltd.
#
# SPDX-License-Identifier: MIT
#
FROM registry.gitlab.apertis.org/infrastructure/apertis-docker-images/v2021-base:latest

ARG DEBIAN_FRONTEND=noninteractive

# Enable and prioritise Atari software sources
COPY atari.list /etc/apt/sources.list.d/
COPY atari /etc/apt/preferences.d/

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y \
      bash                \
      pkg-config          \
      build-essential     \
      libsdl2-dev         \
      libvulkan-dev       \
      libweston-9-dev     \
      libwayland-dev      \
      libgl-dev           \
      libglx-dev          \
      libgtk2.0-dev       \
      libatari-leds-dev   \
      libbz2-dev          \
      libpipewire-0.2-dev \
      libpulse-dev        \
      zlib1g-dev          \
      libsdl2-ttf-dev
## FIXME: Add X11 libraries

