# dumb-init-docker

Dockerfiles for dumb-init on top of various OS dockerfiles.

There are automated builds of these Dockerfiles in the following repositories on [Docker hub](https://hub.docker.com/):

* [joelnb/dumb-init-alpine](https://hub.docker.com/r/joelnb/dumb-init-alpine)
* [joelnb/dumb-init-debian](https://hub.docker.com/r/joelnb/dumb-init-debian)
* [joelnb/dumb-init-ubuntu](https://hub.docker.com/r/joelnb/dumb-init-ubuntu)

These will be updated each time this repository is updated or the underlying images change.

## Why dumb-init?

I think this is best covered by forwarding you to the [dumb-init documentation](https://github.com/Yelp/dumb-init/blob/master/README.md) or the [blog post introducing it](https://engineeringblog.yelp.com/2016/01/dumb-init-an-init-for-docker.html). For some more general reading on why your containers should be using an init system see [this post](https://blog.phusion.nl/2015/01/20/docker-and-the-pid-1-zombie-reaping-problem/) from Phusion which explains the technical details.
