# Snap for Radarr (v3 Legacy)

This is a snap for Radarr, a movie collection manager for Usenet and BitTorrent users.

It is based on a project by Alberto Donato for the [Sonarr](https://sonarr.tv) Smart PVR:

https://github.com/albertodonato/sonarr-snap

This snap only works up to Radar v3 (considered legacy version).

To use the latest Radar versions update to the dotnet snap: <https://github.com/kinekt4/radarr-dotnet>

## Installation

First build:

```bash
    snapcraft --debug
```

Then install:

```bash
    sudo snap install --dangerous radarr_*.snap
```

## Web GUI

The web interface is available at <http:/localhost:7878> after installation.

## More

Please see the [wiki](https://github.com/kinekt4/radarr-snap/wiki) for more information.
