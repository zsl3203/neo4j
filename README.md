# neo4j 安装配置文档
## 1.下载neo4j
```
https://go.neo4j.com/download-thanks.html?edition=community&release=3.5.22&flavour=unix&_ga=2.17540158.622519096.1602571208-674703985.1599616380
```
## 2. 解压缩文件
```
tar -xf neo4j-community-3.5.22-unix.tar.gz
```
## 3. 找到配置文件neo4j.conf
```
cd neo4j-community-3.5.22/conf
```
## 4. 删除54、71、75、79行的#
```
dbms.connectors.default_listen_address=0.0.0.0

dbms.connector.bolt.listen_address=:7687

dbms.connector.http.listen_address=:7474

dbms.connector.https.listen_address=:7473
```

