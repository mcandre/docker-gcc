# docker-gcc - a Docker container for compiling code with gcc

# DOCKER HUB

https://registry.hub.docker.com/u/mcandre/docker-gcc/

# EXAMPLE

```
$ docker run -it -v $(pwd):/mnt mcandre/docker-gcc bash
root@b2b639fe64c0:/# cd /mnt
root@b2b639fe64c0:/mnt# mkdir -p bin/
root@b2b639fe64c0:/mnt# gcc -o bin/hello --static hello.c
root@b2b639fe64c0:/mnt# bin/hello
Hello World!
root@b2b639fe64c0:/mnt# exit
$ ls bin/
hello
```

# REQUIREMENTS

* [Docker](https://www.docker.com/)

## Optional

* [make](http://www.gnu.org/software/make/)
* [Node.js](https://nodejs.org/en/) (for dockerlint)
* [editorconfig-cli](https://github.com/amyboyd/editorconfig-cli) (e.g. `go get github.com/amyboyd/editorconfig-cli`)
* [flcl](https://github.com/mcandre/flcl) (e.g. `go get github.com/mcandre/flcl/...`)
