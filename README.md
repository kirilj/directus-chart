# directus-chart
> A [Helm](https://www.helm.sh/) Chart for [Directus](https://getdirectus.com/)

[![appjumpstart chat][gitter-image]][gitter-url]

## Requirements

Directus requires MySQL (or maybe MariaDB) but this
chart doesn't set this up for you since there is already a stable chart for
[MySQL](https://github.com/kubernetes/charts/tree/master/stable/mysql).

## Configuration

You can copy the default values to a config file, e.g.:

```console
helm inspect values ./directus > directus.yml
```

You can then customize the config values as necessary.

## Installation

```console
helm install --name <release name> -f <config file> --set directus.db.pass=somepass ./directus
```

## Upgrading

```console
helm upgrade <release name> ./directus -f <config file> --set directus.db.pass=somepass
```

&nbsp;

<a href="https://github.com/appjumpstart">
  <img
    alt="AppJumpstart"
    src="https://appjumpstart.nyc3.digitaloceanspaces.com/assets/appjumpstart-transparent.png"
    height="50">
</a>

[gitter-image]: https://img.shields.io/gitter/room/appjumpstart/appjumpstart.svg
[gitter-url]: https://gitter.im/appjumpstart
