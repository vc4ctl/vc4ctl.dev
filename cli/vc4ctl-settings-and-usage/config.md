---
description: Config commands
---

# Config

Change vc4ctl configurations using subcommands like `vc4ctl config add test https://myserver.com 123456`

# Usage

`vc4ctl config SUBCOMMAND`

## add

`vc4ctl config add NAME URL TOKEN`

* `NAME` should be a unique name for this server
* `URL` should be just the host name, with no trailing slash, eg. `https://my.vc4.server.com`
* `TOKEN` should be the token generated using the VC4 web interface
