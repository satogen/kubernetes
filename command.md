# コマンド一覧
## リソースタイプ
リソース一覧を表示できる。
表示されるテキストは３つあるが、どちらもkubectl [command] [TYPE]
のTypeで利用可能。
```bash
kubectl api-resources
```
[ref](https://kubernetes.io/ja/docs/reference/kubectl/)
## get nodeコマンドのオプション
optionにはyaml, json, wideなど指定でき、表示形式を変更できる。
```bash
kubectl get node -o [option] 
```

