## 前端开发环境

### docker 镜像

基于 node 官方镜像，将 npm 目录改成 /.npm，为了后面的持久化。

#### 构建
```
docker build -t fev .
```

### Drun 命令

`docker run` 的简写，快速启动 docker 并运行指定镜像

#### 安装

放到 PATH 下即可

#### 例子
```
drun fev npm install -g @vue/cli

drun fev npm install

drun  -p 8080:8080 fev npm run start
```
