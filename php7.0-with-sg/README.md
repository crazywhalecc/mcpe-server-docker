## Feature
提供了PHP7.2-ZTS版本的SourceGuardian最新版

## 手动build用法
1. 新建文件夹 `mcserver/`， `mcdocker/` ，文件夹名字可自定义
2. 将Dockerfile下载到 `mcdocker/` 目录下，然后 `cd mcdocker`
3. build docker，指令 `sudo docker build -t mcpe .`
4. 将你的核心 `.phar` 文件重命名为 `server.phar` ，丢入 `mcserver` 文件夹。
4. 运行docker，指令： `cd ~/mcserver/ && sudo docker run --rm -it -v $(pwd)/:/mcserver mcpe`

## remote 直接拉镜像
1. 新建文件夹 `mcserver`，并cd进去
4. 将你的核心 `.phar` 文件重命名为 `server.phar` ，丢入 `mcserver` 文件夹。
2. `sudo docker run --rm -it -v $(pwd)/:/mcserver jesse2061/mcpe-server-php7.0-with-sg`
