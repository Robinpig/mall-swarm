


## env


MySQL添加user

```sql
CREATE database mall default character set utf8mb4 collate utf8mb4_unicode_ci;

CREATE USER 'reader'@'%' IDENTIFIED BY '123456';

GRANT ALL PRIVILEGES on *.* TO 'reader'@'%' WITH GRANT OPTION;
```


提前创建network
```shell
docker network create mall
```


copy nginx整个conf目录

ES安装plugin后需要重启
```shell
bin/elasticsearch-plugin install https://get.infini.cloud/elasticsearch/analysis-ik/7.17.3
```


prometheus data需要权限 chmod 777

grafana是3000端口，账密admin/admin

## app

app部署前确保所有prod配置文件加载到nacos

build docker images
```shell
maven install
```

