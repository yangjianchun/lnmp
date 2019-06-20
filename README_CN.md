**[English](README.md)**

## 文档

## 环境需求

1. 安装docker且docker engine至少 `>= 17.06.0+`

2. [安装docker-compose且docker-compose至少 `>= 1.14.0`](https://github.com/docker/compose/releases/tag/1.14.0)

**参见：[Compose file version 3 reference](https://docs.docker.com/compose/compose-file/#reference-and-guidelines)**


## 使用

把 `env-example` 复制为 `.env`，通过运行 `./sync.sh up` 来构建镜像和创建容器。

## docker for linux

在这里，如果你的操作系统是 `Linux` 的话，那么，**建议**修改 `.env` 下的几个配置项

- APP_CODE_PATH_CONTAINER_MODE=:cached

```
docker-compose -f docker-compose.yml up
```

## 关于docker for mac磁盘同步问题
./sync.sh up
```

## 协议

lnmp 的开源协议为 Apache-2.0，详情参见[LICENSE](LICENSE)
