# vcs-build-container

These Docker images provide a compatible build environment for the
Atari VCS. They can be used as the basis for build workflows and
continuous integration for the platform. 

You may want to look at
[bundle-gen](https://github.com/atari-vcs/bundle-gen) for a more
complete VCS build solution based on these containers.

Currently available images:
- `ghcr.io/atari-vcs/vcs-build-container:base`: just the base OS; you can use `apt-get`
  to install additional packages from the Atari VCS and Apertis
  repositories
- `ghcr.io/atari-vcs/vcs-build-container:rust`: the base OS with a
  working (recent) [rust](https://www.rust-lang.org) environment
  pre-installed.
