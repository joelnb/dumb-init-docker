FROM fedora:latest
LABEL maintainer="joelnbarnham@gmail.com"

RUN \
	dnf install -y python-pip && \
	pip install dumb-init && \
	dnf remove -y 'python-pip' && \
	dnf clean -y all && \
	:

ENTRYPOINT ["dumb-init"]
