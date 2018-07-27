### zabbix-docker安装

1. 本地安装docker-compose

```shell
apt installl python-pip
pip install docker-compose
```

2. clone zabbix-docker

```shell
git clone https://github.com/zabbix/zabbix-docker.git
cd zabbix-docker
sed -i '/512M/d'  docker-compose_v2_alpine_mysql_latest.yaml
docker-compose -f docker-compose_v2_alpine_mysql_latest.yaml up -d
```

3. visit url http://hostip

   

   重要数据目录在zbx_env目录

   

