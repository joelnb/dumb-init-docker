FROM alpine:3
LABEL maintainer="joelnbarnham@gmail.com"

RUN \
	apk add --update \
		python3 \
		python3-dev \
		py-pip \
		build-base \
	&& \
	pip install dumb-init && \
	apk del \
		python3 \
		python3-dev \
		py-pip \
		build-base \
	&& \
	rm -rf /var/cache/apk/* && \
	:

ENTRYPOINT ["dumb-init"]
CMD ["/bin/sh"]
