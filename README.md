# 作業 - 6. 架設 Mariadb sql server

[Doc](https://mariadb.com/docs/skysql-previous-release/connect/clients/mariadb-client/)

正常要使用的話應該還要把 config 和 db mount 出來

## install

### client

```
sudo apt install wget

wget https://downloads.mariadb.com/MariaDB/mariadb_repo_setup

echo "3a562a8861fc6362229314772c33c289d9096bafb0865ba4ea108847b78768d2 mariadb_repo_setup" \
    | sha256sum -c -

chmod +x mariadb_repo_setup

sudo ./mariadb_repo_setup \
   --mariadb-server-version="mariadb-10.6"

sudo apt update

sudo apt install mariadb-client
```

## execute

```
mariadb -h localhost -u sam -p
```
