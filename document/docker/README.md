

build docker images
```shell
maven install
```


提前创建network
```shell
docker network create mall
```


env 需要 copy nginx整个conf目录

ES安装plugin后需要重启
```shell
bin/elasticsearch-plugin install https://get.infini.cloud/elasticsearch/analysis-ik/7.17.3
```



app部署前确保所有prod配置文件加载到nacos


