## MySQLのバージョン8のみのComposeファイル
MySQL8.0.33のDocker Composeファイルです。  
port 3306でMySQLのDockerコンテナを用意します。

### ログイン情報  
user: root  
password: password  

### 起動

```shell
$ docker-compose up -d
```

### 停止

```shell
$ docker-compose down
```

### コンテナに入る

```shell
$ docker-compose exec db /bin/bash
```

### Windowsでmy.cnfが読み込めない

```shell
[Warning] World-writable config file '/etc/mysql/my.cnf' is ignored.
```

my.cnfファイルを右クリックして、読み取り専用にする。