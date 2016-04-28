### 機能

Wiki、Jenkins、GitBucketで構成する開発環境を構築する。

### 準備

1.ソース取得

    # git clone https://github.com/saberfrost/tomcat-jenkins-gitbucket

2.コンテナを作成

    # cd tomcat
    # ./build.sh
    # cd ../nginx-fpm
    # ./build.sh
    # cd ../nginx-proxy
    # ./build.sh

### データディレクトリ作成

    # mkdir /var/docker/jenkins
    # mkdir /var/docker/gitbucket
    # mkdir /var/docker/wikitten
    # mkdir /var/docker/www

### 起動

　docker-compose up -d

### dockerコンテナ

[リバースプロキシ](https://hub.docker.com/r/saberfrost/nginx-proxy/)

[PHPサーバ](https://hub.docker.com/r/saberfrost/nginx-fpm/)

[TOMCAT](https://hub.docker.com/r/saberfrost/tomcat-jenkins-gitbucket/)
