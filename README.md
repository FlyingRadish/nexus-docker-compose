# nexus-docker-compose

基于Nexus+Clash的开发环境基础设施，为你的开发加速

## 用途
- 代理公共repo(npm\maven\etc),加速代码构建
- 私有repo
- docker pull镜像代理

## 使用
1. 打开docker-compose.yaml文件，配置clash与nexus的本地映射目录路径
2. 复制clash配置文件到clash目录
3. `docker compose up -d`
4. 打开yacd，配置clash节点
5. 登录nexus，配置http_proxy、https_proxy为`172.50.0.2:7890`
