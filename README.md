# Open Kanban

A simple kanban selfhosted.

Feature list:

* Tasks (with Users, Categories and Priorities)
* Comments
* Filters
* No database support

Original webui code author: https://github.com/scazzy/kanban-board

## LIMITATIONS TO THIS CODE - Comments by Joseph Granata
Unfortunately this software will not run using this README instructions.
Go has changed, and it now does not allow many things this code did, for example:

go get -v github.com/gin-gonic/gin

Does not work instead something like:

go install github.com/gin-gonic/gin@latest

Is needed.

Furthermore the go-assets-builder seems not to work now, or at least it is not clear to me how to properly compile it and use it with this code base.

*I am not yet a Go developer, but I was interested in making this work, after all I am a programmer, but a full update from a Go programmer is needed to make this work again.*


## Screenshot

![image](https://user-images.githubusercontent.com/561184/162066838-df45e389-07c4-49b8-831c-6520d0c79af8.png)

## Building

```bash
go get -v github.com/gin-gonic/gin
go get -v github.com/jessevdk/go-assets-builder

go-assets-builder -s /www -o assets.go www
go build
```
