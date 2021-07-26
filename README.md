# System Tooling with Go

(Loosely) follows the [A Cloud Guru](https://acloud.guru/overview/cc84a84e-c461-4935-90a2-f2127431b855) course by Keith Thompson.

## Setup
* Set env vars in `~/.bashrc`
```bash
# PATH
export GOPATH="${HOME}/go"
export GOROOT="${HOME}/.go"
export PATH="$GOPATH/bin:$PATH"

# go
# https://stackoverflow.com/a/67930263
export GO111MODULE=auto
```

* Install `g` then select latest go version
```bash
curl -sSL https://git.io/g-install | sh -s
```

## Hello, world!
Via [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-build-and-install-go-programs)
```bash
# Run with temp binary
$ go run hello.go
Hello, World!

# Compile for realsies
$ go build -o hello
$ ./hello
Hello, World!

# Move to compiled directory
$ mv hello ../bin
```
