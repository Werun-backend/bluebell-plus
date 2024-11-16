# bluebell 后端代码

## 项目启动

- 需要有 Docker 与 docker-compose 环境
- 在 `bluebell-backend`目录下执行命令，一键通过 `Dockerfile` 打包镜像并进行编排：

```shell
docker-compose up -d
```
- 宿主机访问 http://localhost:8081 查看项目
- 宿主机访问 http://localhost:8081/swagger/index.html 查看接口文档


## docker 部署命令

**构建镜像**
> docker build -t bluebell_app .

**启动容器**
> docker run -d -p 8081:8081 --name bluebell_app bluebell_app

**查看容器日志**
> docker logs -f bluebell_app


