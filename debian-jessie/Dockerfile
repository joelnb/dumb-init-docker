FROM debian:8
LABEL maintainer="joelnbarnham@gmail.com"

RUN \
	export DEBIAN_FRONTEND=noninteractive && \
	apt-get update && \
	apt-get upgrade -y && \
	apt-get install -y \
		build-essential \
		python3-dev \
		python3-pip \
	&& \
	pip3 install dumb-init && \
	apt-get remove -y \
		build-essential \
		python3-dev \
		python3-pip \
	&& \
	apt-get autoremove -y && \
	apt-get clean && \
	rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
	:

ENTRYPOINT ["dumb-init"]
