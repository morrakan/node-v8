# V8 Bindings for Go [![Build Status](https://travis-ci.org/augustoroman/v8.svg?branch=master)](https://travis-ci.org/augustoroman/v8) [![Go Report Card](https://goreportcard.com/badge/github.com/morrakan/node-v8)](https://goreportcard.com/report/github.com/morrakan/node-v8) [![GoDoc](https://godoc.org/github.com/morrakan/node-v8?status.svg)](https://godoc.org/github.com/morrakan/node-v8)

The v8 bindings allow a user to execute javascript from within a go executable.

The bindings are tested to work with several recent v8 builds matching the
Chrome builds 54 - 60 (see the .travis.yml file for specific versions). For
example, Chrome 59 (dev branch) uses v8 5.9.211.4 when this was written.

Note that v8 releases match the Chrome release timeline:
Chrome 48 corresponds to v8 4.8.\*, Chrome 49 matches v8 4.9.\*. You can see
the table of current chrome and the associated v8 releases at:

http://omahaproxy.appspot.com/

#This is a clone of github.com/augustoroman/v8, configured to use pre-compiled v8 for linux64 


# Using a pre-compiled v8

This repository pre-configured to use "libv8-7.0.276.38.0beta1-x86_64-linux.gem", thus, need only:

```bash
go get github.com/morrakan/node-v8

# Run the tests to make sure everything works
cd $GOPATH/src/github.com/morrakan/node-v8
go test
```

## Verifying

You should be done! Try running `go test`

# Reference

Also relevant is the v8 API release changes doc:

https://docs.google.com/document/d/1g8JFi8T_oAE_7uAri7Njtig7fKaPDfotU6huOa1alds/edit

# Credits

This work is based off of several existing libraries:

* https://github.com/fluxio/go-v8
* https://github.com/kingland/go-v8
* https://github.com/mattn/go-v8
