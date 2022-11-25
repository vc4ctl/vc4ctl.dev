---
description: Getting started with the CLI
---

# CLI

## Add a server

Prior to adding a server for control with vc4ctl, an API token must be created using the VC-4 web interface. See the [Crestron VC-4 REST API](https://www.crestron.com/getmedia/29921c49-86df-488c-a63b-ab88620d7175/mg\_pg\_rest-api-crestron-virtual-control) documentation section on Authentication for instructions on adding a token.

Once a token has been created, the following command will add the server configuration and save it for use later:

`vc4ctl config add <name> <url> <token>`

* `<name>` - This must be a unique name for this server
* `<url>` - Full URL to the server, e.g. `https://myVC4server.com`
* \`\<token>\` - Token created using VC-4 UI

The server configuration is stored in `~/.vc4/config.yaml`

### `Example`

`` `vc4ctl config add default https://myvc4server.com 123456` ``

## Choose a server to use

Once a server has been added to the configuration, it can be chosen for use using the following command:

`vc4ctl config use <name>`

* \`\<name>\` - The unique name of the server to use

Once set, all non-config commands will be run using the URL and token set in the configuration.

### Example

`vc4ctl config use default`

## Get all running rooms

Once a server is set for use, a list of all running rooms can be obtained using the following command:

`vc4ctl get rooms`

## Get a single room

Details on a single room can be obtained using the following command:

`vc4ctl get room <roomId>`

* `<roomId>` - The room ID for a room.

### Example

`vc4ctl get room myroom`
