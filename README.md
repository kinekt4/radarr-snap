# Snap for Radarr Smart PVR

This is a snap for the [Radarr](https://radarr.video) Smart PVR.

It is based on a project by Alberto Donato for the [Sonarr](https://radarr.video) Smart PVR:

https://github.com/albertodonato/sonarr-snap

## Installation
This snap has not been published to the [Snapcraft](https://snapcraft.io) store yet.

If/when it does, it can be installed from the store via:

```bash
    sudo snap install radarr
```

## Web GUI

After installing the snap the service web interface will be accessible at
<http:/localhost:7878> by default.

## Storage Configuration

Since the application runs as a confined snap by default, the application will
only be able to access files under `/var/snap/radarr`.  It is also possible to
access storage under `/media` by manually connecting the `removable-media`
interface with

```bash
    sudo snap connect radarr:removable-media
```

It's suggested to create a directory owned by `root` either under
`/var/snap/radarr/common` or under `/media`, after connecting the interface.

*Note*: mount points information won't be displayed by default, as it requires
manually connecting the `mount-observe` interface:

```bash
    sudo snap connect radarr:mount-observe
```


## Build

The snap can be built by simply running:

```bash
    snapcraft --debug
```

Once, built, install the snap with:

```bash
    sudo snap install --dangerous radarr_*.snap
```
