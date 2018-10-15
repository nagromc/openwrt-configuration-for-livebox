# OpenWRT configuration for Livebox

This is an OpenWRT minimal working configuration for Orange's Livebox as per described in a dedicated [lafibre.info \[FR\] thread](https://lafibre.info/remplacer-livebox/remplacement-de-la-livebox-par-un-routeur-openwrt-18-dhcp-v4v6-tv/) for the following routers:

- Linksys WRT1900ac v2.0
- Linksys WRT610N v1.0

Once the script is executed, your router will be given an IPv4 and IPv6.

You are welcome to open a Pull Request on this repo to share your knowledge.

## Requirements

You need a Unix-like environment to run the installer. The installation script has **not** been tested on Windows (Cygwin).

## Installation

To configure your router, just set the `$CLEARTEXT_FTI` variable with your own `fti` value.

```shell-session
$ export CLEARTEXT_FTI=fti/xxxxxxx
```

Then, depending on which router you want to configure (`wrt1900acv2` or `wrt610n`), run the following command from your own machine:

```shell-session
$ ./install -r wrt1900acv2
```
