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

