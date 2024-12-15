# コマンド一覧
## リソースタイプ
リソース一覧を表示できる。
表示されるテキストは３つあるが、どちらもkubectl [command] [TYPE]
のTypeで利用可能。
```bash
kubectl api-resources
```
[ref](https://kubernetes.io/ja/docs/reference/kubectl/)
## get コマンドのオプション
optionにはyaml, json, wideなど指定でき、表示形式を変更できる。
```bash
kubectl get node -o [option] 
```

## Name空間とPoｄの確認
```bash
kubectl get pod --all-namespaces
```
名前空間を指定してかつ、PODを確認する
```
kubectl get pod -n [name]
```

## ノードの詳細確認
IPアドレスやSystemInfoが表示される。
メモリのリミットやAllocateの情報がある。
GETよりも詳細の情報がわかる
```bash
kubectl describe node docker-desktop
```

下記のコマンドで特定のPrefixを持っているNamePaceの情報を取得
```bash
kubectl describe ns [prefix]
```

特定のPODが動作していない場合などは下記のコマンド
```bash
kubectl describe pod [pod] -n [name]
```