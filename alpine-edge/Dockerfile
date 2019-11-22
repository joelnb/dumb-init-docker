FROM alpine:edge
LABEL maintainer="joelnbarnham@gmail.com"

RUN \
	apk add --update \
		python2 \
		python2-dev \
		py2-pip \
		build-base \
	&& \
	pip install dumb-init && \
	apk del \
		python2 \
		python2-dev \
		py2-pip \
		build-base \
	&& \
	rm -rf /var/cache/apk/* && \
	:

ENTRYPOINT ["dumb-init"]
CMD ["/bin/sh"]
