# logstash
自定义ES模板的logstash

`index-mapper.json`: 该文件是自定义的映射模板

`mysqltoes.conf`:该文件是全量更新的配置文件

`mysqltoes_update.conf`:该文件是增量更新的配置文件



运行：

```bash
# 全量更新
cd 到logstash的根目录
.\bin\logstash -f mysqltoes.conf
# 增量更新
.\bin\logstash -f mysqltoes_update.conf
```

> `注意`：
>
> 修改对应的配置文件里的数据库链接以及账号密码
>
> 修改对应的配置文件里的sql
