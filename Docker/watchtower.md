---
title: Docker watchtower升级容器
description: 
published: 1
date: 2022-10-21T18:20:20.612Z
tags: docker, watchtower, upgrade
editor: markdown
dateCreated: 2022-08-24T19:45:45.599Z
---

### Docker升级容器

1. 通过watchtower升级container:

   ```bash
    docker run --rm \
    -v /var/run/docker.sock:/var/run/docker.sock \
    containrrr/watchtower \
    --run-once -c container_name
   ```
   * -c 升级后删除旧的docker镜像
   * container_name 为需要被升级的容器名
