# ruimarinho/z-way

A Z-Way server docker image.

[![build status][travis-image]][travis-url]
[![ruimarinho/z-way][docker-pulls-image]][docker-hub-url] [![ruimarinho/z-way][docker-stars-image]][docker-hub-url] [![ruimarinho/z-way][docker-size-image]][docker-hub-url] [![ruimarinho/z-way][docker-layers-image]][docker-hub-url]

## Supported tags and respective `Dockerfile` links

- `2.3.6`, `2`, `latest` ([2/Dockerfile](https://github.com/ruimarinho/docker-z-way/blob/master/2/Dockerfile))

This image will be automatically updated whenever there is an update to the base image (`ubuntu:rolling`).

## What is Z-Way?

_from [Z-Wave.me](https://www.z-wave.me/index.php?id=22):_

Every Smart Home in general and every Z-Wave Network in particular is controlled by a central controller and regardless whether this is a large PC or a small router box, there is a software that implements the communication and control function.

Z-Wave.me's flagship software to control Z-Wave networks is called Z-Way. Z-Way was the very first Z-Wave control software certified by the Z-Wave Alliance back in March 2011.

### Integration with Z-Wave.me (ZME) UZB1 Stick

If you own a ZME UZB1 Stick, you can load it on the Z-Way server using device mapping:

```sh
❯ docker run --rm -it -p 8083:8083 --device=/dev/ttyACM0 ruimarinho/z-way
```

By loading your UZB1 Stick, you will be able to update its bootloader and firmware versions.

## Usage

### How to use this image

This image contains the server binary from the Z-Way software and by default runs the `z-way-server`.

```sh
❯ docker run --rm -it -p 8083:8083 ruimarinho/z-way
```

Now go to http://127.0.0.1:8083 to open the UI.

## Supported Docker versions

This image is officially supported on Docker version 1.12, with support for older versions provided on a best-effort basis.

## License

[License information](https://github.com/ruimarinho/docker-z-way/blob/master/LICENSE) for the [ruimarinho/docker-z-way][docker-hub-url] docker project.

[docker-hub-url]: https://hub.docker.com/r/ruimarinho/z-way
[docker-layers-image]: https://img.shields.io/imagelayers/layers/ruimarinho/z-way/latest.svg?style=flat-square
[docker-pulls-image]: https://img.shields.io/docker/pulls/ruimarinho/z-way.svg?style=flat-square
[docker-size-image]: https://img.shields.io/imagelayers/image-size/ruimarinho/z-way/latest.svg?style=flat-square
[docker-stars-image]: https://img.shields.io/docker/stars/ruimarinho/z-way.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/ruimarinho/docker-z-way.svg?style=flat-square
[travis-url]: https://travis-ci.org/ruimarinho/docker-z-way
