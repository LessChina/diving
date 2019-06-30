# diving

Using diving you can analyze docker image on the website. It use [dive](https://github.com/wagoodman/dive) to get the analyzed information.


The first time may be slow, because it pulls the image first.

![Image](.data/demo.gif)


## Installation

```
docker run -d --restart=always \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -p 7001:7001 \
  vicanso/diving
```
---

## Other Tools

回顾下之前介绍的几款：

**【推荐】用来探索`docker`镜像背后的每一层文件系统，以及发现缩小镜像体积方法的命令行工具（启动命令：`dive 镜像名`）**
> <https://github.com/LessChina/dive>

**【推荐】不改变内容缩小Docker镜像**：
> <https://github.com/lotapp/docker-slim>

**【推荐】基于`Docker`的持续集成平台**
> <https://github.com/lotapp/drone>

**Docker终端管理工具**
> <https://github.com/lotapp/docui>
