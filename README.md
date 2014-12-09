# Beego Dev

## Introduction

Build beego development environment with one command. Docker handles these for you.

* Install Golang 1.4
* Configurate GOPATH and PATH
* Install [beego](https://github.com/astaxie/beego) and [bee](https://github.com/beego/bee)
* Automatically load the code from local

No need to install go at all and it allows you to write code with your favorite IDE.

## Usage

Initialize beego project with `git clone`, `go get` or `bee new`. Then run the docker command.

```
docker run -i -t --net=host -v /home/tobegit3hub/seagull:/go/src/tobegit3hub/seagull tobegit3hub/beego_dev
```

The option `--net=host` allows you to access beego application within docker container. And `-v` will load your code from local. Make sure put your project in `/go` which is the GOPATH of container.



