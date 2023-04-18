# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages
RUN sudo apt-get -y update && sudo apt-get -y dist-upgrade

# Install xz-utils
RUN sudo apt-get install -y xz-utils

# Install novnc
RUN sudo apt install -y novnc

# Run noVNC
RUN sudo novnc --listen 6081 --vnc localhost:5901
