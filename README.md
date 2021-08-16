# jianmu-runner-image-build

#### 介绍
用于通过Dockerfile创建镜像，并推送至镜像仓库  

#### 参数说明  
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

