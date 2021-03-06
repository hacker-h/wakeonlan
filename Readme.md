# Wakeonelan
This is a simple python alpine based docker image with the wakeonlan tool installed.

[![Build Status](https://travis-ci.org/hacker-h/wakeonlan.svg?branch=master)](https://travis-ci.org/hacker-h/wakeonlan)

# Usage
```
docker run --net=host hackerh/wakeonlan wakeonlan -i <BROADCAST_IP> -p <PORT> <MAC_ADDRESS>
```

# Example Usage
```
docker run --net=host hackerh/wakeonlan wakeonlan -i 192.168.0.255 -p 9 25:3E:BF:3E:28:D9
```

# Notice
Attaching `--net=host` for the container is mandatory, as WOL packets (layer 2) can't pass the docker network bridge.

# References
pipeline code:
https://dev.to/zeerorg/build-multi-arch-docker-images-on-travis-5428

architecture/variant syntax for docker manifests:
https://github.com/moby/moby/issues/34875
