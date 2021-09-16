# jianmu-runner-image-build

#### 介绍
用于通过Dockerfile创建镜像，并推送至镜像仓库  

#### 输入参数 
```
JIANMU_DOCKER_USERNAME: docker仓库用户  
JIANMU_DOCKER_PASSWORD: docker仓库用户密码  
JIANMU_IMAGE_NAME: docker镜像名  
JIANMU_IMAGE_TAG: docker镜像tag
JIANMU_DOCKER_FILE: Dockerfile文件路径
JIANMU_DOCKER_BUILD_PATH: 镜像构建目录
JIANMU_WORKSPACE: 执行构建命令的目录
JIANMU_CMD_PRE: 构建前执行命令
JIANMU_CMD_POST: 构建后执行命令
```

#### 构建docker镜像
```
# 创建docker镜像
docker build -f dockerfilexxx -t jianmudev/jianmu-runner-docker:${version}

# 上传docker镜像
docker push jianmudev/jianmu-runner-docker:${version}
```

#### 用法
创建镜像
```
docker run --rm \
  -e JIANMU_DOCKER_USERNAME=xxx \
  -e JIANMU_DOCKER_PASSWORD=xxx \
  -e JIANMU_IMAGE_NAME=xxx \
  -e JIANMU_IMAGE_TAG=xxx \
  -e JIANMU_DOCKER_FILE=xxx \
  -e JIANMU_DOCKER_BUILD_PATH=xxx \
  -e JIANMU_DOCKER_BUILD_PATH=xxx \
  -e JIANMU_WORKSPACE=xxx \
  -e JIANMU_CMD_PRE=xxx \
  -e JIANMU_CMD_POST=xxx \
  jianmudev/jianmu-runner-docker:${version}
```
