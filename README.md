## これは何をしようとして作った？

wordpressのデザインをテストしようとして作りました。

dockerでwordpressが起動します。

また、phpmyadminも動いているので、データベースの操作もやりやすくしています。


## アクセス

### wordpress

http://ip_address:8080

### phpmyadmin

http://ip_address:8081


## 起動

以下で起動します。

docker-compose up

## 特徴

大容量のテストデータをインポートするため、php.iniを読み込ませるようにしています。

また、データベースは永続化していません。コンテナが無くなれば、データも無くなります。