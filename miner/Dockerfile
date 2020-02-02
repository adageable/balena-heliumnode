# Set the base image (note: stretch-20180426 is latest fixed image)
FROM balenalib/raspberrypi4-64-debian-node:latest-buster-build

# Dockerfile author / maintainer
MAINTAINER Name <adageable@gmail.com>

# set bash as the default shell for all dockerfile RUN commands
SHELL ["/bin/bash", "-c"]

#RUN echo $'\
#APT::Install-Recommends "0";\n\
#APT::Install-Suggests "0";\n' \
#> /etc/apt/apt.conf.d/10norecommends

# ------------------------------------------------------------------------
# packages - baseline additions for all platforms (development, test, and final production build)
# ------------------------------------------------------------------------
RUN apt-get -y --no-install-recommends update && \
apt-get -y --no-install-recommends upgrade
