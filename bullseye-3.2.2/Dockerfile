ARG DOCKER_REGISTRY=public.aml-repo.cms.waikato.ac.nz:443/
FROM ${DOCKER_REGISTRY}debian:bullseye

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get -y install \
          gdal-bin \
          git && \
    rm -rf /var/lib/apt/lists/*

COPY bash.bashrc /etc/bash.bashrc
