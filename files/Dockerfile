# Dockerfile

# Author       : Adityasinh Sodha
# Github       : https://github.com/WorkofAditya
# Messenger    : https://m.me/Adityasinhji
# Email        : work.adityasodha@gmail.com
# Main Language: Python

# Import main images

# OS
FROM debian:latest
# Main Language
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/KasRoudra/WorkofAditya"

# Working directory
WORKDIR /Phisherman/
# Add files 
ADD . /Phisherman

# Installing packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "phisherman.py", "--noupdate"]
