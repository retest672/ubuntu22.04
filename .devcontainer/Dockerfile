# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages
RUN sudo apt-get -y update && sudo apt-get -y dist-upgrade

# Install pip3 because (apparently) there is no pip installed in Ubuntu 22.04 Image
RUN sudo apt-get install -y python3-pip
