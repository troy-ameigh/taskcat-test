FROM python:3.8.13-alpine3.15

LABEL maintainer="Tony Vattathil tonynv@amazon.com"

# Version
LABEL version=production

# Operating Systems
LABEL container-os=python

RUN apk update && apt install -y gcc
RUN pip3 install taskcat --upgrade \
&& pip3 install --index-url https://test.pypi.org/simple/ taskcat  --no-cache-dir --force --upgrade --no-deps

# Set the work directory
WORKDIR /mnt
