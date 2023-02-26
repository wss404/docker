# docker-by-hand
手写docker
开发过程中使用docker环境调试，命令如下：
```
# 构建docker镜像
docker build -t golang:lab
# 进入容器shell
docker run -it --rm --privileged --name golab -v /Users/imte/code/repository/docker:/go/src -w /go/src golang /bin/bash
# 直接运行go run main.go
docker run -it --rm --privileged --name golab -v /Users/imte/code/repository/docker:/go/src -w /go/src golang:lab go run main.go
```
