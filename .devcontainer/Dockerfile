# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages
RUN sudo apt-get -y update && sudo apt-get -y dist-upgrade

# Install firefox-esr
RUN sudo apt-get install -y xfce4 xfce4-goodies

# Install firefox-esr
RUN DEBIAN_FRONTEND=noninteractive sudo apt-get install -y firefox-esr

# Install xz-utils
RUN sudo apt-get install -y xz-utils

# Install snap store
RUN sudo apt install -y snapd

# Install noVNC
RUN sudo snap install -y novnc

# Add snap path to $PATH variable
RUN export PATH=/snap/bin:$PATH

# Run noVNC
RUN sudo novnc --listen 6081 --vnc localhost:5901
