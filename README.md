## 准备
### 运行镜像打包disconf

```
docker build -t scoop/disconf-build .
```

### 运行镜像容器，将打包的目录挂载到本地

```
docker run -v ${pwd}/disconf-rd/working:/home/work/dsp/disconf-rd/working -v ${pwd}/disconf-rd/config:/home/work/dsp/disconf-rd/online-resources --name disconf-build scoop/disconf-build
```

### 整理sql文件

将https://github.com/knightliao/disconf/tree/master/disconf-web/sql下sql整理成一个sql文件disconf\sql\0-init.sql

```
0-init_table.sql
1-init_data.sql
201512/20151225.sql
20160701/20160701.sql
```
## 运行

```
docker-compose up -d
```