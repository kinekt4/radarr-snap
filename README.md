# Snap for Radarr

This is a snap for Radarr, a movie collection manager for Usenet and BitTorrent users.

It is based on a project by Alberto Donato for the [Sonarr](https://sonarr.tv) Smart PVR:

https://github.com/albertodonato/sonarr-snap

## Installation

### Snap Store

**Note**: This snap has not been published to the [Snapcraft Snap Store](https://snapcraft.io/store) yet.

Therefore, the following will not work yet.

```bash
    sudo snap install radarr
```

### Build

The snap can be built by simply running:

```bash
    snapcraft --debug
```

Once built, install the snap with:

```bash
    sudo snap install --dangerous radarr_*.snap
```

## Web GUI

The web interface is available at [http:/localhost:7878](http:/localhost:7878) after installation.

## More

Please see the [wiki](https://github.com/kinekt4/radarr-snap/wiki) for more information.
