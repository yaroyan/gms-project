dockerコンテナ内からパッケージインストールに失敗する場合に試してみること

dotnetのイメージのコンテナをビルドすると
コンテナ内部からdotnet new installコマンドの実行に失敗して難儀する。

/etc/docker/daemon.json
```
{"dns":["8.8.8.8", "8.8.4.4"]}
```

cat /etc/resolv.conf

```
nameserver 1.1.1.1
```