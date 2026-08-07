# tammy-snap

Snapcraft packaging for [Tammy](https://tammy.connect2x.de), a fast and secure
Matrix messenger built on the decentralized Matrix protocol.

This repository only contains the `snapcraft.yaml` and supporting files used
to build and publish the `tammy` snap. The Tammy application itself is
developed at [gitlab.com/connect2x/tammy](https://gitlab.com/connect2x/tammy);
this packaging pulls the latest released Linux build directly from that
project's releases.

## Building

```
snapcraft pack
```

This produces a `tammy_<version>_amd64.snap` file that can be installed with:

```
sudo snap install --dangerous tammy_<version>_amd64.snap
```

## Installing from the Snap Store

Once published:

```
sudo snap install tammy
```
