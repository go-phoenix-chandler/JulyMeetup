# Contribute to Go

## Step 1

* https://golang.org/doc/contribute.html

## Step 2

* `go get -u golang.org/x/tools/cmd/go-contrib-init`
* `git clone --depth 1 https://go.googlesource.com/go ~/golang`
* `cd ~/golang`
* `go-contrib-init`
* if Brew -> `export GOROOT_BOOTSTRAP=/usr/local/Cellar/go/1.8.x/libexec`
* else -> `export GOROOT_BOOTSTRAP=/usr/local/go`
* `cd src`
* `./buildall.bash`
* `alias dev-go='~/golang/bin/go'`
* `godoc -goroot='/path/to/golang' -http=:6060`
* `GOROOT='' dev-go test <pkg>`

## Step 3

* Add code
* `git add . && git change`
* Add commit message. Prefix message with package change was made in. E.g. "os: some message here"
* `git mail`. This will upload your code to Gerrit and provide you a link to the page for the code review.

## Adding New Files

Include the following header:

```
// Copyright 2017 The Go Authors. All rights reserved.
// Use of this source code is governed by a BSD-style
// license that can be found in the LICENSE file.
```
