## ׼��
### ���о�����disconf

```
docker build -t scoop/disconf-build .
```

### ���о����������������Ŀ¼���ص�����

```
docker run -v ${pwd}/disconf-rd/working:/home/work/dsp/disconf-rd/working -v ${pwd}/disconf-rd/config:/home/work/dsp/disconf-rd/online-resources --name disconf-build scoop/disconf-build
```

### ����sql�ļ�

��https://github.com/knightliao/disconf/tree/master/disconf-web/sql��sql�����һ��sql�ļ�disconf\sql\0-init.sql

```
0-init_table.sql
1-init_data.sql
201512/20151225.sql
20160701/20160701.sql
```
## ����

```
docker-compose up -d
```