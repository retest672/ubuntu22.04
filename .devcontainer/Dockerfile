# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages
RUN sudo apt-get -y update && sudo apt-get -y dist-upgrade

# Install xz-utils
RUN sudo apt-get install -y xz-utils

# Install snap store
RUN sudo apt install -y snapd

# Activate snapd service
RUN sudo systemctl enable --now snapd.socket

# Install noVNC
RUN sudo snap install -y novnc

# Add snap path to $PATH variable
RUN export PATH=/snap/bin:$PATH

# Run noVNC
RUN sudo novnc --listen 6081 --vnc localhost:5901
