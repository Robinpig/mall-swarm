

build docker images
```shell
maven install
```


提前创建network
```shell
docker network create mall
```


env 需要 copy nginx整个conf目录

ES安装plugin
```shell
./bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v7.17.3/elasticsearch-analysis-ik-7.17.3.zip
```



app部署前确保所有prod配置文件加载到nacos


