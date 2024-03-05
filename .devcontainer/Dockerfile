# Use Ubuntu 22.04 Image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Update all packages and install python (3.11) full suite
RUN sudo apt-get -y update && sudo apt-get -y dist-upgrade
RUN sudo apt-get -y install software-properties-common
RUN sudo add-apt-repository universe multiverse
RUN sudo add-apt-repository ppa:deadsnakes/ppa
RUN sudo apt -y install python3.11-full python3.11-lib2to3 python3.11-venv python3.11-tk python3.11-dev python3.11-distutils
RUN curl -sS https://bootstrap.pypa.io/get-pip.py | python3.11
