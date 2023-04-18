# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages
RUN sudo apt-get update && sudo apt-get dist-upgrade

# Install firefox-esr
RUN DEBIAN_FRONTEND=noninteractive sudo apt-get install -y firefox-esr

# Install xz-utils
RUN sudo apt-get install -y xz-utils

# Install snap store
RUN sudo apt install snapd
