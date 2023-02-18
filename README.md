# docker-spigot-api-doc

本文档资源来自 BukkitAPI 汉化组（https://github.com/BukkitAPI-Translation-Group），本项目仅做封装整理，无法提供关于API的任何咨询和技术支持！

# 官方资源

* 1.19.2 文档：[https://bukkit.windit.net/javadoc/](https://bukkit.windit.net/javadoc/)
* 1.19.2 英文原版：[https://hub.spigotmc.org/javadocs/bukkit/](https://hub.spigotmc.org/javadocs/bukkit/)
* BukkitAPI 汉化组：[https://github.com/BukkitAPI-Translation-Group](https://github.com/BukkitAPI-Translation-Group)

# 如何使用

## 方式1：常规web环境

常规web环境是指如：`lnmp/lamp` 或 `宝塔面板` 这种，此处仅做简单说明，不进行详细的图文说明！

* 建立一个新站点
* 将 `src` 上传到站点根目录

## 方式2：容器化部署

容器化部署是指基于 docker 技术，快速基于做好的 `镜像` 生成一个 `容器`，开箱即用的意思！需保证服务器已经装好了 docker 相关服务！

### 方式1：docker-compose 方式部署（推荐）

```yml
version: '3'
services:
  docker-spigot-api-doc:
    image: timoprince/docker-spigot-api-doc
    container_name: docker-spigot-api-doc
    ports:
      - 8801:80
    restart: always
```

### 方式2：docker 命令行方式部署

```shell
docker run -itd --name=docker-spigot-api-doc -p 8801:80 timoprince/docker-spigot-api-doc
```
