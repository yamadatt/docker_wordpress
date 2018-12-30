## 起動

以下で起動します。‐dオプションをつけるのもあり。

docker-compose up

## wordpressにログイン

以下のユーザとパスワードでログインします。

* ユーザ:user
* パスワード:user

## wordpress.sqlの編集

wordpress.sqlにIPアドレス（'192.168.150.130'）が記述されているので、以下のように環境に合わせて書き換える。

grep -l '192.168.150.130' wordpress.sql | xargs sed -i.bak -e 's/192.168.150.130/192.168.1.254/g'
