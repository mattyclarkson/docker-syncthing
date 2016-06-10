# Alpine Syncthing Docker Container

[![Docker Stars](https://img.shields.io/docker/stars/bambucha/syncthing.svg)](https://registry.hub.docker.com/u/bambucha/syncthing/)
[![Docker Pulls](https://img.shields.io/docker/pulls/bambucha/syncthing.svg)](https://registry.hub.docker.com/u/bambucha/syncthing/)
[![Docker Layers](https://img.shields.io/imagelayers/layers/bambucha/syncthing/latest.svg)](https://registry.hub.docker.com/u/bambucha/syncthing/)
[![Docker Size](https://img.shields.io/imagelayers/image-size/bambucha/syncthing/latest.svg)](https://registry.hub.docker.com/u/bambucha/syncthing/)

## Usage

```shell
docker run \
    --user 1000:1000 \
    --publish 8384:8384 \
    --publish 22000:22000 \
    --publish 21027:21027/udp \
    --volume `pwd`/config:/config \
    --volume `pwd`/Sync:/mnt/Sync \
    --name syncthing \
    --restart always \
    --detach \
    bambucha/syncthing
```

## License

[The MIT License](LICENSE)
