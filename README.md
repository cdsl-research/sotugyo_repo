# sotugyo_repo

リバースプロキシを構築するために作成したマニフェストファイルである．
### nginx-configmap.yaml
configmapのマニフェストファイルである．主にNginxの設定ファイルを定義するために使用される．
テスト用に作成したWebサーバにプロキシするように書かれている．

### nginx-deployment.yaml
deploymentのマニフェストファイルである．Podの数を管理するために使用される．

### nginx-servce.yaml
servceのマニフェストファイルである．Podの公開・接続の方法を管理する．

## 使用方法
以下のコマンドを打つ．
```
kubectl apply -f ./nginx-configmap/*
```
＊プロキシ先のWebサーバがなければ正常に動作しない．
