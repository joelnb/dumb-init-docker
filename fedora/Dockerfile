FROM fedora:latest
LABEL maintainer="joelnbarnham@gmail.com"

RUN \
	dnf install -y 'dnf-command(copr)' && \
	dnf copr enable -y alsadi/dumb-init && \
	dnf install -y dumb-init && \
	dnf copr disable -y alsadi/dumb-init && \
	dnf remove -y 'dnf-command(copr)' && \
	dnf clean -y all && \
	:

ENTRYPOINT ["dumb-init"]