Nyanstagram for iOSアプリ用のダッシュボードです。  
[Dashing](http://shopify.github.com/dashing) フレームワークでできています。

必要なもの
----
* Heroku Toolbelt (https://toolbelt.heroku.com/)
* Ruby 2.0.0
* Google Analyticsのアカウント
* Nendのアカウント

環境変数の設定
----
Google Analytics, Nend から情報を取得するための環境変数を設定してください。

開発環境
```
# Google Analytics
$ export GA_USERNAME=example@qnyp.com
$ export GA_PASSWORD=enter-your-passward
$ export GA_UA_CODE=UA-********-1

# Nend
$ export NEND_URL=https://www.nend.net/admin/login/********=
$ export NEND_MAIL=example@qnyp.com
$ export NEND_PASSWORD=enter-your-passward
```

Heroku
```
# Google Analytics
$ heroku config:add GA_USERNAME=example@qnyp.com
$ heroku config:add GA_PASSWORD=enter-your-passward
$ heroku config:add GA_UA_CODE=UA-********-1

# Nend
$ heroku config:add NEND_URL=https://www.nend.net/admin/login/********=
$ heroku config:add NEND_MAIL=example@qnyp.com
$ heroku config:add NEND_PASSWORD=enter-your-passward
```

開発環境で確認
----
`dashing`コマンドで起動します

```
$ bundle exec dashing start
```

デプロイ
----
```
$ git push heroku master
```
