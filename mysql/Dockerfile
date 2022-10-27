FROM mysql:8.0

# MySQLのローカルの設定ファイルをコンテナにコピー
COPY ./my.cnf /etc/mysql/conf.d/my.cnf

# init.sqlをコンテナの/docker-entrypoint-init.db.dと共有
COPY ./init-prd.sql /docker-entrypoint-initdb.d