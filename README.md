# Golang build tags

Golang build tags are a way to include or exclude certain
portions of code from the final binary during the build process. 
They are specified using a comment of the form "`// +build tag1 tag2`" 
at the top of a file, and they can also be used to specify the operating
system, architecture, or other build constraints. 
The `go build `command can then be run with the `-tags` flag to specify 
which tags should be included or excluded. For example, if you have a build
tag named `"unix"` in your code, you can use` go build -tags unix` to include
that code only when building for the unix platform.

## Compiling this example
```shell
$ go build -tags "debug"
```

