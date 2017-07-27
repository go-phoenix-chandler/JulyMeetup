# Contribute to Go

* https://golang.org/doc/contribute.html
* `go get -u golang.org/x/tools/cmd/go-contrib-init`
* `git clone --depth 1 https://go.googlesource.com/go ~/golang`
* `cd ~/golang`
* `go-contrib-init`

* if Brew -> `export GOROOT_BOOTSTRAP=/usr/local/Cellar/go/1.8.x/libexec`
* else -> `export GOROOT_BOOTSTRAP=/usr/local/go`
* `./buildall.bash`
* `alias dev-go='/Users/bdowns/golang/bin/go'`

If having to compile Go, we'll need to run `GOROOT='' dev-go test bytes` to test

## Adding New Files

Include the following header:

```
// Copyright 2017 The Go Authors. All rights reserved.
// Use of this source code is governed by a BSD-style
// license that can be found in the LICENSE file.
```
